---
title: "DataLoadHdFile"
description: "Loads data set properties from a DIAdem Dat data file."
---

# DataLoadHdFile

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataLoadHdFile

Loads data set properties from a DIAdem Dat data file.

## Signature

```python
dd.DataLoadHdFile(DataFile)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Before you call the command <a href="../dataloadsel/">DataLoadSel</a>, you must execute the commands <a href="../hdload/">HdLoad</a> or <a href="./">DataLoadHdFile</a> to load the channel properties. Otherwise DIAdem cannot specify any channel names.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DataFile</td>
<td>Specifies the name of the current data file.<div id="exp_DataFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.DataLoadHdFile("Drive.dat") #Read header file
dd.DataFileLoadSel("Drive.dat","DAT","[1]/[2]")
```

---

*Source: `ComOff/DataLoadHdFile.htm`*
