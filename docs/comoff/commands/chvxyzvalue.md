---
title: "ChVXYZValue"
description: "Specifies for an x/y-coordinate the x/y/z-values on a surface that either correspond to the next value on the surface, the interpolated surface value, or the ma"
---

# ChVXYZValue

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChVXYZValue

Specifies for an x/y-coordinate the x/y/z-values on a surface that either correspond to the next value on the surface, the interpolated surface value, or the maximum or the minimum of the surface. You can specify the 3D data as a triplet or as a matrix.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>You can determine the associated row number using the <a href="../chnfindxyzvalue/">ChnFindXYZValue</a> function.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the triple or the matrix.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the triple or the matrix.</td></tr>
<tr><td width="150"><em>Z</em></td>
<td>Specifies the data channel that contains the z-values of the triple or the first data channel with the z-values of the matrix.</td></tr>
<tr><td width="150">D3DataType</td>
<td>Specifies whether the data is available in triplet or matrix form.<div id="exp_D3DataType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Triplet"</pre></donottranslate></td>
<td>Triplet structure</td></tr>
<tr><td width="150"><donottranslate><pre>"Matrix"</pre></donottranslate></td>
<td>Matrix structure</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">XSearchValue</td>
<td>Specifies the x-value of the point which the condition refers to.<div id="exp_XSearchValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">YSearchValue</td>
<td>Specifies the y-value of the point which the condition refers to.<div id="exp_YSearchValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">D3SearchMode</td>
<td>Specifies a condition.<div id="exp_D3SearchMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NearestValue"</pre></donottranslate></td>
<td>Next value</td></tr>
<tr><td width="150"><donottranslate><pre>"Interpolation"</pre></donottranslate></td>
<td>Interpolated value</td></tr>
<tr><td width="150"><donottranslate><pre>"AbsoluteMax"</pre></donottranslate></td>
<td>Absolute minimum</td></tr>
<tr><td width="150"><donottranslate><pre>"AbsoluteMin"</pre></donottranslate></td>
<td>Absolute maximum</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant variable</a> type. Receives a three dimensional field. The field receives the x-, y-, and z-values which meet the specified condition.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChVXYZValue.htm`*
