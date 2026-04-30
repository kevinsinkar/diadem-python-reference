---
title: "ValEqualGT"
description: "Checks whether the first numeric value is greater than or equal to the second numeric value:"
---

# ValEqualGT

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ValEqualGT

Checks whether the first numeric value is greater than or equal to the second numeric value:

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The comparison uses the internal DIAdem algorithm to determine whether the values are equal. DIAdem only uses the significant digits of a number. For example, the expression <span class="Monospace">ValEqualGT(1,1.000000000000001)</span> returns the value <span class="Monospace">TRUE</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Value</td>
<td>Specifies a numeric value.<div id="exp_Value">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">Value</td>
<td>Specifies the comparative value.<div id="exp_Value__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean</a> type.</td></tr>
</table>
</div>

---

*Source: `ComOff/ValEqualGT.htm`*
