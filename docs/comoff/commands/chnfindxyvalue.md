---
title: "ChnFindXYValue"
description: "Specifies for an x/y-coordinate the point on a curve that corresponds to either the next value, the interpolated value, or a maximum or a minimum. The command s"
---

# ChnFindXYValue

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFindXYValue

Specifies for an x/y-coordinate the point on a curve that corresponds to either the next value, the interpolated value, or a maximum or a minimum. The command specifies the row number of a channel pair whose values meet the specified condition. You can specify the 3D data as a triplet or as a matrix.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>You can determine the relevant x-value and y-value using the <a href="../chvxyvalue/">ChVXYValue</a> function.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the value pair.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values.</td></tr>
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
<tr><td width="150">D2SearchMode</td>
<td>Specifies a condition.<div id="exp_D2SearchMode">
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
<tr><td width="150"><donottranslate><pre>"LocalMax"</pre></donottranslate></td>
<td>Local maximum</td></tr>
<tr><td width="150"><donottranslate><pre>"LocalMin"</pre></donottranslate></td>
<td>Local minimum</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Longinteger-variable</a> type. Receives the row number of a channel pair whose values meet the given condition.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnFindXYValue.htm`*
