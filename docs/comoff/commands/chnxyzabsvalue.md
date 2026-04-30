---
title: "ChnXYZAbsValue"
description: "Calculates the resultant acceleration for an x, y, and z-channel."
---

# ChnXYZAbsValue

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnXYZAbsValue

Calculates the resultant acceleration for an x, y, and z-channel.

## Signature

```python
return_value = dd.ChnXYZAbsValue( X , Y , Z , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the descriptions of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the acceleration values in x-direction.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration values in y-direction.</td></tr>
<tr><td width="150"><em>Z</em></td>
<td>Specifies the data channel containing the acceleration values in z-direction.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnXYZAbsValue.htm`*
