---
title: "ChnConvertUnitToUnitSet"
description: "Valid names: ChnConvertUnitToUnitSet, ChnConvertToUnitSet"
---

# ChnConvertUnitToUnitSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertUnitToUnitSet

Valid names: ChnConvertUnitToUnitSet, ChnConvertToUnitSet

## Signature

```python
dd.ChnConvertUnitToUnitSet(ChnList, UnitSet, IgnoreUnknownUnits)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif" style="width: 26"/></td><td><strong>Note  </strong>If you use the <span class="Monospace">ChnConvertToUnitSet</span> command with the parameter setting <span class="Monospace">IgnoreUnkownUnits = True</span> in a user command, and call the command from an event or a layout instead of from a script, DIAdem displays a warning message. If you want to suppress these warning messages, use the <span class="Monospace">ChnConvertToUnitSet</span> command with the parameter setting <span class="Monospace">IgnoreUnkownUnits = False</span>, and enclose this command with <span class="Monospace">On Error Resume Next</span> ... <span class="Monospace">On Error Goto 0</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">UnitSet</td>
<td>Specifies the unit set.<div id="exp_UnitSet">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">IgnoreUnknownUnits</td>
<td>Specifies whether DIAdem ignores unknown units (<span class="Monospace">TRUE</span>) or whether DIAdem throws an error (<span class="Monospace">FALSE</span>).<div id="exp_IgnoreUnknownUnits">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertUnitToUnitSet.htm`*
