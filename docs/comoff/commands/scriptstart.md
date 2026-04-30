---
title: "ScriptStart"
description: "Valid names: ScriptStart, VBSStart"
---

# ScriptStart

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ScriptStart

Valid names: ScriptStart, VBSStart

## Signature

```python
dd.ScriptStart(FileDlgName, [VBSProcName], [AutoObjLetOpen])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path in the <span class="Monospace">FileDlgName</span> variable, DIAdem loads the file from the SCRIPT user folder or saves the file in the SCRIPT user folder. If you do not enter a filename extension, DIAdem determines the filename extension from the variable <a href="../../../varoff/variables/filedlgfilt/">FileDlgFilt</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>When the <span class="Monospace">ScriptStart</span> command is called, DIAdem also executes the main section of the subscript and initializes the variables. The command then runs the specified subroutine.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  When the <span class="Monospace">ScriptStart</span> command is called, you cannot debug the routines, transfer parameters, or access the script variables. You can use only DIAdem variables or user variables to transfer values. Therefore, use the <a href="../scriptinclude/">ScriptInclude</a> command instead. If you use the <span class="Monospace">ScriptInclude</span> command instead of the <span class="Monospace">ScriptStart</span> command, you can <a href="#" data-unresolved="1">speed up scripts</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../scriptinclude/">ScriptInclude</a> command instead of the <span class="Monospace">ScriptStart</span> command when you extend scripts. The following table describes the various application options. Call <span class="Monospace">ScriptInclude</span> only once at the beginning of a script. Do not call the <span class="Monospace">ScriptInclude</span> command in loops.<table class="Borderless">
<tr>
<td><strong>ScriptStart</strong></td>
<td><strong>ScriptInclude</strong></td><td> </td>
</tr>
<tr>
<td> </td>
<td>X</td><td>When you use transfer parameters</td>
</tr>
<tr>
<td> </td>
<td>X</td><td>When you use return values</td>
</tr>
<tr>
<td> </td>
<td>X</td>
<td>When you debug calls in another script</td>
</tr>
<tr>
<td> </td>
<td>X</td>
<td>When you use name spaces</td>
</tr>
<tr>
<td> </td>
<td>X</td>
<td>When you use objects and variables from another script</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you start a script as program parameter</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you specify menus, buttons, and other controls to start a script</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you call scripts via OLE</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you cancel the started script or local error for this script</td>
</tr>
</table>
</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileDlgName</td>
<td>Specifies a file. You also can specify the path and the filename extension.<div id="exp_FileDlgName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path in the <span class="Monospace">FileDlgName</span> variable, DIAdem loads the file from the SCRIPT user folder or saves the file in the SCRIPT user folder. If you do not enter a filename extension, DIAdem determines the filename extension from the variable <a href="../../../varoff/variables/filedlgfilt/">FileDlgFilt</a>.</td></tr></table>
</div></td></tr>
<tr><td width="150">[VBSProcName]</td>
<td>Specifies the name of a subroutine. By default the <span class="Monospace">VBSProcName</span> variable contains an empty text. For Python scripts, the command ignores this parameter.<div id="exp_VBSProcName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 255 characters</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[AutoObjLetOpen]</td>
<td>For future extensions.</td></tr>
</table>
</div>

---

*Source: `ComOff/ScriptStart.htm`*
