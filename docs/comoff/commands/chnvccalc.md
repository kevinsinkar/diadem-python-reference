---
title: "ChnVCCalc"
description: "Calculates the Viscous Criterion value (VC), which is an injury criterion for the chest area."
---

# ChnVCCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnVCCalc

Calculates the Viscous Criterion value (VC), which is an injury criterion for the chest area.

## Signature

```python
return_value = dd.ChnVCCalc( XW , Y , ResultChannel , CrashDummyConst, VCScalefactor, VCDirective)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="../../../inavidata/properties/idiademproperty-value/">Value for Property</a> property to request or to set channel properties.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">VC criterion</a> for further information, such as background, input value, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the amplitude values of the unfiltered deformation signal in meters.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">CrashDummyConst</td>
<td>Specifies the deformation constant (chest depth) of the dummy in millimeters.<div id="exp_CrashDummyConst">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">VCScalefactor</td>
<td>Specifies the scaling factor of the dummy.<div id="exp_VCScalefactor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= VCScalefactor &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">VCDirective</td>
<td>Specifies the directive or the law for the VC calculation.<div id="exp_VCDirective">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"PIAS"</pre></donottranslate></td>
<td>PIAS (outdated)</td></tr>
<tr><td width="150"><donottranslate><pre>"ECE_94"</pre></donottranslate></td>
<td>ECE_94</td></tr>
<tr><td width="150"><donottranslate><pre>"SAE_J1727"</pre></donottranslate></td>
<td>SAE_J1727</td></tr>
<tr><td width="150"><donottranslate><pre>"EuroNCAP"</pre></donottranslate></td>
<td>EuroNCAP</td></tr>
<tr><td width="150"><donottranslate><pre>"PRE_FILTERED"</pre></donottranslate></td>
<td>Pre-filtered</td></tr>
</table>
</td></tr>
</table>
<p class="body">Use the <span class="Monospace">PRE_FILTERED</span> setting when the dummy provides previously filtered input signals.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnVCCalc.htm`*
