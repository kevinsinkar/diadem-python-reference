---
title: "ScriptCmdRemove"
description: "Removes a script that contains user commands. You cannot use the commands defined in this script later in DIAdem. DIAdem deletes all variables generated with Gl"
---

# ScriptCmdRemove

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ScriptCmdRemove

Removes a script that contains user commands. You cannot use the commands defined in this script later in DIAdem. DIAdem deletes all variables generated with GlobalDim .

## Signature

```python
dd.ScriptCmdRemove(ScriptFile)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Only use the <span class="Monospace">ScriptCmdRemove</span> command at the end of a script. Then execute the command <a href="../scriptcmdreset/">ScriptCmdReset</a> for DIAdem to restart the script engine.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the page <a href="#" data-unresolved="1">Using User Commands</a> for more information.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ScriptFile</td>
<td>Specifies the name of a script file.<div id="exp_ScriptFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ScriptCmdRemove.htm`*
