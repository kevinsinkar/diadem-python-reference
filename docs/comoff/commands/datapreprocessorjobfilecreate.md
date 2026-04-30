---
title: "DataPreProcessorJobFileCreate"
description: "Creates a job file for the data preparation."
---

# DataPreProcessorJobFileCreate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataPreProcessorJobFileCreate

Creates a job file for the data preparation.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ProcessFileLocation</td>
<td>Specifies the path where DIAdem saves the job file. DIAdem creates the filename automatically. Select this path for job files in the data preparation. As soon as data preparation finds new job files in this folder, it processes this file automatically.<div id="exp_ProcessFileLocation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PathsToBeProcessed</td>
<td>Specifies an array that contains the names of the files or paths which the DataFinder is to reindex. You must specify the files with the complete path. If the array contains more than 100 file or path entries, the command creates a further job file. The specified files or folders must be in the search areas of the Data Preparation instance.<div id="exp_PathsToBeProcessed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ProcessPathType]</td>
<td>Specifies whether file paths or folder paths are contained in the <span class="Monospace">PathsToBeProcessed</span> variable. The default value of the variable is <span class="Monospace">"Folder"</span>.<div id="exp_ProcessPathType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"File"</pre></donottranslate></td>
<td>File</td></tr>
<tr><td width="150"><donottranslate><pre>"Folder"</pre></donottranslate></td>
<td>Folders</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String</a> type.</td></tr>
</table>
</div>

## Python example

```python
sFolder = "C:\\Users\\Public\\Documents\\National Instruments\\dd.Data Preprocessor\\Data\\"
sJobFileLocation  = "C:\\Users\\Public\\Documents\\National Instruments\\dd.Data Preprocessor\\"

sFileOrFolderToBeProcessed = []
sFileOrFolderToBeProcessed.append(sFolder + "TR_M17_QT_42-1.tdms")
sFileOrFolderToBeProcessed.append(sFolder + "TR_M17_QT_42-2.tdms")
sFileOrFolderToBeProcessed.append(sFolder + "TR_M17_QT_42-4.tdms")
sFileOrFolderToBeProcessed.append(sFolder + "TR_M17_QT_42-5.tdms")
sFirstJobFileName = dd.DataPreProcessorJobFileCreate(sJobFileLocation, sFileOrFolderToBeProcessed, "File")
print(sFirstJobFileName)
```

---

*Source: `ComOff/DataPreProcessorJobFileCreate.htm`*
