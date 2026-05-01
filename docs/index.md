---
title: "DIAdem Python Scripting Reference"
---

# DIAdem Python Scripting Reference

Consolidated from the **DIAdem 2026 Q2** (Edition April 2026) help bundle. 13,431 elements across 29 sources. Generated 2026-05-01 21:59 UTC.

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
