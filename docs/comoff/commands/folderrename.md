---
title: "FolderRename"
description: "Renames a folder."
---

# FolderRename

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FolderRename

Renames a folder.

## Signature

```python
dd.FolderRename(FSSourceName, FSTargetName, [FSProgressBar])
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
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem renames read-only folders on your computer without requesting confirmation. DIAdem does not rename read only folders in a network.</td></tr></table>
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
dd.FolderRename("C:\\Old_Folder","C:\\MyFolder")
```

---

*Source: `ComOff/FolderRename.htm`*
