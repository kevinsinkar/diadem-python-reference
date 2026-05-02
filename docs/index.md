---
title: "DIAdem Python Scripting Reference"
---

# DIAdem Python Scripting Reference

Consolidated from the **DIAdem 2026 Q2** (Edition April 2026) help bundle. 13,431 elements across 29 sources. Generated 2026-05-02 02:38 UTC.

## Getting started

```python
import win32com.client
# On current DIAdem 2026 installs the working ProgID is "DIAdem.TOCmd".
# The CHM-era docs often show "DIAdem.Application"; that ProgID is no longer
# registered on a fresh install. Use DIAdem.TOCmd.
dd = win32com.client.Dispatch("DIAdem.TOCmd")
result = dd.DataFileLoad("C:/Example.tdm")
for ch_group in dd.Data.Root.ChannelGroups:
    print(ch_group.Name)
```

Throughout this reference the conventional handle name `dd` is used in examples. Pass DIAdem enum constants by reading them through the same handle (e.g. `dd.eExportToCSV`) or by their integer value.

Topics whose source CHM did not include a Python tab were machine-translated from VBScript and carry a yellow callout above the example.

## Runtime gotchas

Three behaviours of DIAdem's COM dispatch that aren't obvious from the topic pages themselves but matter once you start scripting against a real DIAdem install:

### 1. The dispatch surface is panel-conditional

Top-level singletons like `dd.Report`, `dd.Navigator`, `dd.View`, and `dd.Calculate` are exposed by DIAdem's TOCmd dispatch only when their corresponding **panel is active in DIAdem**. If you spawn DIAdem purely by `Dispatch("DIAdem.TOCmd")` from a headless context, the early dispatch may resolve only `dd.Data` (the always-loaded core), and accesses like `dd.Report` will raise `AttributeError: DIAdem.TOCmd.Report` until the REPORT panel initializes.

**Practical advice:** for any non-trivial automation, **launch DIAdem manually first** and let its UI fully load before running your script. Once DIAdem is up with all panels visible, `dd.Report`, `dd.Navigator`, `dd.View`, etc. all resolve normally.

If you must drive DIAdem entirely from Python, you can force-load panels via the secondary `DIAdem.TOCommand` bridge:

```python
import win32com.client
bridge = win32com.client.Dispatch("DIAdem.TOCommand")
for panel in ("NAVIGATOR", "VIEW", "ANALYSIS", "REPORT", "SCRIPT"):
    bridge.CmdExecuteSync(f'Call WndShow("{panel}","Show")')
dd = win32com.client.Dispatch("DIAdem.TOCmd")  # full surface now visible
```

Note: pywin32 caches negative attribute lookups, so if you got an `AttributeError` once, the next access in the same `dd` instance returns the cached miss. Recover by re-Dispatching `dd` after the panel is loaded.

### 2. `dd.Visible = True` does not work

The Visible property is read-only on the TOCmd dispatch &mdash; you can't make a hidden DIAdem visible from Python. If you need DIAdem on screen, launch it manually (or via `subprocess.Popen`) before dispatching.

### 3. Closing DIAdem mid-script breaks subsequent COM calls

If DIAdem.exe exits while your script holds a `dd` reference, every subsequent attribute access raises `(-2147023174, 'The RPC server is unavailable.')`. There is no recovery short of relaunching DIAdem and re-Dispatching. Wrap long-running scripts in a guard that re-launches if needed, or check `dd.Data` periodically to detect a dead handle early.

### 4. Some global script variables are read-only on TOCmd

DIAdem's internal script engine treats many global variables (e.g. `ChnEventResultList`, `D3StrucOut`, `ChnEventList1`, `PrinterName`, `CalcQuantityBased`, `ClassNo`, `GHdChnNo`, `D3GridCalcAll`, `D3IsoLineSource`, `PrintName`) as direct assignment targets. The CHM examples show this style:

```python
# Inside DIAdem's built-in script editor (works there):
ChnEventResultList = "/MyResult"
```

From external Python via `DIAdem.TOCmd`, those properties are read-only and `dd.ChnEventResultList = "..."` raises a property-set error. Use the secondary `DIAdem.TOCommand` bridge instead, which exposes typed variable setters:

```python
import win32com.client

bridge = win32com.client.Dispatch("DIAdem.TOCommand")
dd     = win32com.client.Dispatch("DIAdem.TOCmd")

# String-typed:
bridge.TextVarSet("ChnEventResultList", "/MyResult")
# Integer-typed:
bridge.IntegerVarSet("ClassNo", 10)
# Boolean-typed:
bridge.BoolVarSet("CalcQuantityBased", True)
# Float-typed:
bridge.DoubleVarSet("MyDouble", 3.14)
# Or, for any type, evaluate VBS in-engine:
bridge.CmdExecuteSync('ClassNo = 10')
```

After the bridge sets the variable, call the corresponding analysis command on `dd` as documented &mdash; the command will read the variable from DIAdem's script-engine globals.

## Browse

| Section | Source CHM | Elements |
| --- | --- | ---: |
| [Application & Script](scripting/index.md) | `Scripting.chm` | 113 |
| [Commands - Offline (Script Engine)](comoff/index.md) | `ComOff.chm` | 722 |
| [Commands - Online (DAC)](comonl/index.md) | `ComOnl.chm` | 246 |
| [NAVIGATOR / Data Portal / Data Finder](scriptnavi/index.md) | `ScriptNavi.chm` | 811 |
| [INaviData (Data Model Interfaces)](inavidata/index.md) | `Inavidata.chm` | 265 |
| [TDM Scripting](tdmscript/index.md) | `TDMScript.chm` | 36 |
| [TDM Context](tdmcontext/index.md) | `TDMcontext.chm` | 104 |
| [REPORT Object Model](reportapi/index.md) | `ReportApi.chm` | 2,941 |
| [VIEW Object Model](scriptview/index.md) | `Scriptview.chm` | 1,115 |
| [Global Script Variables (Offline)](varoff/index.md) | `VarOff.chm` | 3,211 |
| [Global Script Variables (Online)](varonl/index.md) | `VarOnl.chm` | 890 |
| [Online Package Variables](pkvaronl/index.md) | `PkVarOnl.chm` | 277 |
| [DataPlugin Authoring](dataplugin/index.md) | `DataPlugin.chm` | 313 |
| [Unit Catalog Scripting](scriptunitcatalog/index.md) | `ScriptUnitCatalog.chm` | 111 |
| [SUD Dialog Editor Scripting](sudref/index.md) | `Sudref.chm` | 1,561 |
| [Context Menu Scripting](contextmenu/index.md) | `ContextMenu.chm` | 14 |
| [Toolbar Manager Interface](tobarmanagerint/index.md) | `ToBarManagerInt.chm` | 164 |
| [JSON Parser](jsonparser/index.md) | `JsonParser.chm` | 7 |
| [OLE Automation](ole/index.md) | `OLE.chm` | 51 |
| [E-Mail Service](emailservice/index.md) | `EMailService.chm` | 18 |
| [LabVIEW Helper](lvhelper/index.md) | `LVHelper.chm` | 24 |
| [Parallel Process Control](parallelprocesscontrol/index.md) | `ParallelProcessControl.chm` | 28 |
| [System Information](systeminfo/index.md) | `SystemInfo.chm` | 12 |
| [IValueUnit](ivalueunit/index.md) | `IValueUnit.chm` | 5 |
| [ICalculationSet](icalculationset/index.md) | `ICalculationSet.chm` | 143 |
| [ICANConverter](icanconverter/index.md) | `ICANConverter.chm` | 104 |
| [File Tagging](filetagging/index.md) | `FileTagging.chm` | 31 |
| [DAC Block: Alarm](gfsalarm/index.md) | `Gfsalarm.chm` | 86 |
| [DAC Block: VBS-Driver](gfsvbsdr/index.md) | `Gfsvbsdr.chm` | 28 |
