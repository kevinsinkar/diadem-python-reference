---
title: "ExtProgram"
description: "Starts an external program."
---

# ExtProgram

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ExtProgram

Starts an external program.

## Signature

```python
dd.ExtProgram(ExtProgramName, ExtProgramArg, [ ExtProgramHide ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If the <span class="Monospace">ExtProgramName</span> variable is empty and the <span class="Monospace">ExtProgramArg</span> variable contains a filename with the extension, DIAdem tries to start the application linked to this file.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem does not wait for the external program to execute. It continues the calling script.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ExtProgramName</td>
<td>Specifies the name of an external program including the path.<div id="exp_ExtProgramName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ExtProgramArg</td>
<td>Specifies the parameters that DIAdem uses to start an external program.<div id="exp_ExtProgramArg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ExtProgramHide]</td>
<td>Specifies whether DIAdem starts the external program with a visible window (FALSE) or not (TRUE). By default DIAdem displays the window.<div id="exp_ExtProgramHide">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ExtProgram("cmd.exe","/c del C:\\test.abc", True)
```

```python
dd.ExtProgram("","C:\\test.docx")
```

---

*Source: `ComOff/ExtProgram.htm`*
