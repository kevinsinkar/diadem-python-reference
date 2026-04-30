---
title: "DataFinderIndexJobFileCreate"
description: "Creates a job file for DataFinders."
---

# DataFinderIndexJobFileCreate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFinderIndexJobFileCreate

Creates a job file for DataFinders.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">JobFileLocation</td>
<td>Specifies the path where DIAdem saves the job file. DIAdem creates the filename automatically. You select this path for job files in a DataFinder instance. As soon as the DataFinder instance finds new job files in this folder, it processes these files automatically.<div id="exp_JobFileLocation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PathsToBeIndexed</td>
<td>Specifies a data field that contains the names of the files or paths which DataFinder is to reindex. You must specify the files with the complete path. If the array contains more than 100 file or path entries, the command creates a further job file. The specified files or folders must be contained in the search areas of the DataFinder instance.<div id="exp_PathsToBeIndexed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[IndexPathType]</td>
<td>Specifies whether file paths or folder paths are contained in the <span class="Monospace">PathsToBeIndexed</span> variable. The default value of the variable is <span class="Monospace">"Folder"</span>.<div id="exp_IndexPathType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"File"</pre></donottranslate></td>
<td>File</td></tr>
<tr><td width="150"><donottranslate><pre>"Folder"</pre></donottranslate></td>
<td>Folder</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String variable</a> type. Contains the name of the first job file.</td></tr>
</table>
</div>

## Python example

```python
sFolder = "C:\\Users\\Public\\Documents\\National Instruments\\DataFinder\\Data\\"
sJobFileLocation  = "C:\\Users\\Public\\Documents\\National Instruments\\DataFinder\\"

sFileOrFolderToBeIndexed = []
sFileOrFolderToBeIndexed.append(sFolder + "TR_M17_QT_42-1.tdms")
sFileOrFolderToBeIndexed.append(sFolder + "TR_M17_QT_42-2.tdms")
sFileOrFolderToBeIndexed.append(sFolder + "TR_M17_QT_42-4.tdms")
sFileOrFolderToBeIndexed.append(sFolder + "TR_M17_QT_42-5.tdms")
sFirstJobFileName = dd.DataFinderIndexJobFileCreate(sJobFileLocation, sFileOrFolderToBeIndexed, "File")
dd.MsgBoxDisp(sFirstJobFileName)
```

---

*Source: `ComOff/DataFinderIndexJobFileCreate.htm`*
