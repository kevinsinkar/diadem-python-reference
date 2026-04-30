---
title: "DataFileCopy"
description: "Copies .tdm , .tdms , or .dat type DIAdem files and the associated binary files containing the bulk data. If you save the data file to another target folder, DI"
---

# DataFileCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileCopy

Copies .tdm , .tdms , or .dat type DIAdem files and the associated binary files containing the bulk data. If you save the data file to another target folder, DIAdem does not automatically copy the video files of the video channels, nor does it change the associated relative paths.

## Signature

```python
dd.DataFileCopy(FSSourceName, FSTargetPath, [FSProgressBar])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The page <a href="#" data-unresolved="1">Loading Bulk Data - General</a> contains important information on the extended loading behavior of TDM and TDMS files.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FSSourceName</td>
<td>Specifies the source file or source folder for DIAdem file and folder commands.<div id="exp_FSSourceName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div></td></tr>
<tr><td width="150">FSTargetPath</td>
<td>Specifies target folders for DIAdem file and folder commands.<div id="exp_FSTargetPath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[FSProgressBar]</td>
<td>Specifies whether the progress bar, which the operating system displays for long operations, is visible. If you assign the value <span class="Monospace">TRUE</span> to the <span class="Monospace">FSProgressBar</span> variable, DIAdem does not display the progress bar. The default value for the <span class="Monospace">FSProgressBar</span> variable is <span class="Monospace">FALSE</span>.<div id="exp_FSProgressBar">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.DataFileCopy(dd.DataLibrPath + "Example.tdm", dd.DataReadPath, False)
```

---

*Source: `ComOff/DataFileCopy.htm`*
