---
title: "ChnDeltaCalc"
description: "Calculates the difference between two successive channel values."
---

# ChnDeltaCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDeltaCalc

Calculates the difference between two successive channel values.

## Signature

```python
return_value = dd.ChnDeltaCalc( Y , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The result is <span class="Monospace">NoValue</span> if one of the channel values is <span class="Monospace">NoValue</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The result channel is one value shorter than the input channel.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values you want to calculate.</td></tr>
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

*Source: `ComOff/ChnDeltaCalc.htm`*
