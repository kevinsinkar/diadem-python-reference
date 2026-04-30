---
title: "DataFileMove"
description: "Moves .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. If you save the data file to another target folder, D"
---

# DataFileMove

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DataFileMove

Moves .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. If you save the data file to another target folder, DIAdem does not automatically copy the video files of the video channels, nor does it change the associated relative paths.

## Signature

```python
dd.DataFileMove(FSSourceName, FSTargetName, [FSProgressBar])
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
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you use the <span class="Monospace">FSTargetName</span> variable in the <a href="../datafilecopy/">DataFileCopy</a> command, you only can assign one path to the variable. If you use the <span class="Monospace">FSTargetName</span> variable in the <a href="../datafilerename/">DataFileRename</a> command, you only can assign one filename without an extension to the variable.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you use the <span class="Monospace">DataFileMove</span> command, the following errors may occur:<ul><li>
<p class="Body">The specified target path does not exist.</p></li>
<li>
<p class="Body">The <span class="Monospace">FSSourceName</span> source contains wildcards, but the target <span class="Monospace">FSTargetName</span> contains a filename instead of a folder.</p></li>
<li>
<p class="Body">The <span class="Monospace">FSSourceName</span> source contains wildcards that do not match any source file.</p></li></ul><p class="Body">The <span class="Monospace">DataFileMove</span> command terminates the action the first time an error occurs. DIAdem does not undo actions it performed before the error occurred. If you use the command for read-only files that are in a local folder, DIAdem does not display an error message. If you use the command for read-only files that are in a network, DIAdem displays an error message.</p>
</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Regardless of which filename extension you specify for the <span class="Monospace">FSSourceName</span> variable, DIAdem only moves DAT files together with the respective binary files. DIAdem ignores all other file types when you use the <span class="Monospace">DataFileMove</span> command.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../filemove/">FileMove</a> command to move files.</td></tr></table>
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
<tr><td width="150">FSTargetName</td>
<td>Specifies target folders or target files for DIAdem file and folder commands.<div id="exp_FSTargetName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you use the <span class="Monospace">FSTargetName</span> variable in the <a href="../datafilecopy/">DataFileCopy</a> command, you only can assign one path to the variable. If you use the <span class="Monospace">FSTargetName</span> variable in the <a href="../datafilerename/">DataFileRename</a> command, you only can assign one filename without an extension to the variable.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
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
dd.DataFileMove("C:\\DIAdem\\*.*","D:\\Target\\")
```

---

*Source: `ComOff/DataFileMove.htm`*
