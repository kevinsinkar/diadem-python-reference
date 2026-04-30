---
title: "ScriptCmdAdd"
description: "Registers a script that contains user commands. Use user commands to add your own commands to DIAdem or to change existing commands."
---

# ScriptCmdAdd

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ScriptCmdAdd

Registers a script that contains user commands. Use user commands to add your own commands to DIAdem or to change existing commands.

## Signature

```python
dd.ScriptCmdAdd(ScriptFile, [ ScriptAddMode ])
```

## Notes

<div markdown="1">
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
<tr><td width="150">[ScriptAddMode]</td>
<td>Specifies how DIAdem registers the user command.<div id="exp_ScriptAddMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"temporary"</pre></donottranslate></td>
<td>Removes the user command after the command ScriptCmdReset was executed.</td></tr>
<tr><td width="150"><donottranslate><pre>"permanent"</pre></donottranslate></td>
<td>Permanent for one DIAdem session (default setting)</td></tr>
<tr><td width="150"><donottranslate><pre>"persistent"</pre></donottranslate></td>
<td>Persistent for several DIAdem sessions</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ScriptCmdAdd.htm`*
