---
title: "ChnFIR100Calc"
description: "Use this command for digital signal filtering."
---

# ChnFIR100Calc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFIR100Calc

Use this command for digital signal filtering.

## Signature

```python
return_value = dd.ChnFIR100Calc( XW , Y , ResultChannel , ResultChannel , Fir100RemoveBias)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">FIR 100 Filters</a> for further information such as background, input value, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">Fir100RemoveBias</td>
<td>Specifies whether DIAdem eliminates the bias in FIR100 filtering. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not remove the bias.<div id="exp_Fir100RemoveBias">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnFIR100Calc.htm`*
