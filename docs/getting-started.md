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

DIAdem is a Windows **COM Automation server** with the registered ProgID
`DIAdem.Application`. From any Windows process you can hand Windows that
ProgID and Windows hands you back a connection to a (possibly hidden)
running DIAdem instance. From Python this is one line via
[`pywin32`](https://pypi.org/project/pywin32/):

```python
import win32com.client
dd = win32com.client.Dispatch("DIAdem.Application")
```

`dd` is now a remote control. Every attribute lookup is a COM call into
the running DIAdem process; results come back as native Python objects
(numbers, strings) or further Dispatch handles for objects.

## A first session

```python
import win32com.client

dd = win32com.client.Dispatch("DIAdem.Application")

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
  `Dispatch("DIAdem.Application")`.
- **`obj`** in a method or property signature stands in for whatever
  interface object the method is called on (e.g. `obj.Add(...)` on an
  `IChannelGroups` collection).
- DIAdem **enum constants** (names beginning with a lower-case `e`) are
  read off the same Dispatch handle: `dd.eExportToCSV`,
  `dd.eGroupChnTimeRel`, etc. They evaluate to integers; passing the
  integer literal directly works too.
- Optional VBScript parameters are marked `[Like_This]` in the original
  signature; in Python they're regular keyword arguments you can omit.
