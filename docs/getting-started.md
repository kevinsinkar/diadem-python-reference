---
title: "Getting started"
---

# Getting started with DIAdem from Python

## What this is

A consolidated, Python-only reference for the DIAdem COM Automation API,
extracted from the DIAdem help bundle. Every command, method, property,
object, event, and global script variable that DIAdem documents is here,
with the Python example DIAdem itself ships in its help topics. Topics whose
source did not include a Python tab carry a machine-translated example with
a clearly marked callout.

## How DIAdem exposes itself

DIAdem is a Windows **COM Automation server**. On current DIAdem 2026
installs the working ProgID is **`DIAdem.TOCmd`**. (The CHM-era documentation
often shows `DIAdem.Application`; that ProgID is no longer registered on a
fresh DIAdem 2026 install — `DIAdem.TOCmd` points at the same coclass and
exposes the same surface.) From any Windows process you hand Windows the
ProgID and Windows hands you back a connection to a (possibly hidden)
running DIAdem instance. From Python this is one line via
[`pywin32`](https://pypi.org/project/pywin32/):

```python
import win32com.client
dd = win32com.client.Dispatch("DIAdem.TOCmd")
```

`dd` is now a remote control. Every attribute lookup is a COM call into
the running DIAdem process; results come back as native Python objects
(numbers, strings) or further Dispatch handles for objects.

## A first session

```python
import win32com.client

dd = win32com.client.Dispatch("DIAdem.TOCmd")

# Load a TDM file into the Data Portal
elements = dd.DataFileLoad("C:/Data/Example.tdm")

# Compute the average of every loaded channel into a result channel
dd.ChnAverage(elements, "/Average")

# Walk the data model
for grp in dd.Data.Root.ChannelGroups:
    for ch in grp.Channels:
        print(grp.Name, ch.Name, ch.Properties("unit_string").Value)

# Save and quit
dd.DataFileSave("C:/Out/result.tdm")
dd.Quit()
```

## Conventions in this reference

- **`dd`** is the conventional handle name for the Dispatch returned by
  `Dispatch("DIAdem.TOCmd")`.
- **`obj`** in a method or property signature stands in for whatever
  interface object the method is called on (e.g. `obj.Add(...)` on an
  `IChannelGroups` collection).
- DIAdem **enum constants** (names beginning with a lower-case `e`) are
  read off the same Dispatch handle: `dd.eExportToCSV`,
  `dd.eGroupChnTimeRel`, etc. They evaluate to integers; passing the
  integer literal directly works too.
- Optional VBScript parameters are marked `[Like_This]` in the original
  signature; in Python they're regular keyword arguments you can omit.

## Runtime gotchas

Four behaviours of DIAdem's COM dispatch that aren't obvious from the topic
pages but matter once you start scripting against a real DIAdem install:

### 1. The dispatch surface is panel-conditional

Top-level singletons (`dd.Report`, `dd.Navigator`, `dd.View`, `dd.Calculate`)
are exposed by DIAdem's TOCmd dispatch only when their corresponding panel
is active in DIAdem. If you spawn DIAdem purely by `Dispatch("DIAdem.TOCmd")`
from a headless context, only `dd.Data` (the always-loaded core) may resolve;
`dd.Report` etc. will raise `AttributeError: DIAdem.TOCmd.Report`.

**Practical advice:** for any non-trivial automation, **launch DIAdem
manually first** and let its UI fully load. Once DIAdem is up with all
panels visible, every documented top-level attribute resolves normally.

If you must drive DIAdem entirely from Python, force-load panels via the
secondary `DIAdem.TOCommand` bridge:

```python
import win32com.client

bridge = win32com.client.Dispatch("DIAdem.TOCommand")
for panel in ("NAVIGATOR", "VIEW", "ANALYSIS", "REPORT", "SCRIPT"):
    bridge.CmdExecuteSync(f'Call WndShow("{panel}","Show")')

dd = win32com.client.Dispatch("DIAdem.TOCmd")  # full surface now visible
```

Note: pywin32 caches negative attribute lookups, so once a `dd.X` access
fails it returns the cached miss until the dispatch is recreated.

### 2. `dd.Visible = True` does not work

The Visible property is read-only on the TOCmd dispatch. To make DIAdem
visible, launch it manually (or via `subprocess.Popen`) before dispatching.

### 3. Closing DIAdem mid-script breaks subsequent calls

If DIAdem.exe exits while your script holds a `dd` reference, every later
attribute access raises `(-2147023174, 'The RPC server is unavailable.')`.
Recovery requires relaunching DIAdem and re-Dispatching from scratch.

### 4. Some global script variables are read-only on TOCmd

Many DIAdem global script variables that act as input parameters for
analysis commands (e.g. `ChnEventResultList`, `D3StrucOut`,
`ChnEventList1`, `PrinterName`, `CalcQuantityBased`, `ClassNo`,
`GHdChnNo`, `D3GridCalcAll`, `D3IsoLineSource`, `PrintName`) are read-only
on `DIAdem.TOCmd`. The CHM examples show direct assignment style:

```python
# Inside DIAdem's built-in script editor (works there):
ChnEventResultList = "/MyResult"
```

From external Python, use the `DIAdem.TOCommand` bridge's typed setters:

```python
import win32com.client

bridge = win32com.client.Dispatch("DIAdem.TOCommand")
dd     = win32com.client.Dispatch("DIAdem.TOCmd")

bridge.TextVarSet("ChnEventResultList", "/MyResult")  # string vars
bridge.IntegerVarSet("ClassNo", 10)                    # integer vars
bridge.BoolVarSet("CalcQuantityBased", True)           # boolean vars
bridge.DoubleVarSet("MyDouble", 3.14)                  # float vars

# Or, for any type, evaluate VBS in DIAdem's script engine:
bridge.CmdExecuteSync('ClassNo = 10')

# Then call the analysis command on dd as documented; it reads the
# variable from DIAdem's script-engine globals.
dd.ChnEventCompareChnEQ(...)
```
