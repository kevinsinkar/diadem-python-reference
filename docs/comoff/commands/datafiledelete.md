---
title: "DataFileDelete"
description: "Deletes .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. If you delete the data file, DIAdem does not automa"
---

# DataFileDelete

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileDelete

Deletes .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. If you delete the data file, DIAdem does not automatically delete the video files of the video channels as well.

## Signature

```python
dd.DataFileDelete(FSSourceName, [FSPreserveUndo], [FSProgressBar])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify a path, DIAdem searches for the file or the folder in the NAVIGATOR user and library path.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>DIAdem deletes local read-only files without a confirmation prompt. DIAdem does not delete read-only files in a network.</td>
</tr>
</table>
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
<tr><td width="150">[FSPreserveUndo]</td>
<td>Specifies whether DIAdem moves files and folders into the recycle bin or deletes them irretrievably. The default value is <span class="Monospace">FALSE</span> which specifies that DIAdem deletes the files irrevocably.<div id="exp_FSPreserveUndo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
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
if dd.FilEx(dd.DataReadPath + "Example.dat") :
    dd.DataFileDelete(dd.DataReadPath + "Example.dat ",True)
```

---

*Source: `ComOff/DataFileDelete.htm`*
