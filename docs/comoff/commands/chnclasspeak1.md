---
title: "ChnClassPeak1"
description: "Calculates the classification with the peak value method I."
---

# ChnClassPeak1

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnClassPeak1

Calculates the classification with the peak value method I.

## Signature

```python
return_value = dd.ChnClassPeak1( Y , ResultChannel , ResultChannel , ClassMeth1, FrequencyType, Hysteresis, ClassRefLine, [OpenBoundClass])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To include all the values of a function in the classification, the bottom limit value of the first class interval must be smaller than the smallest value of the function you want to classify.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To include all the values of a function in the classification, the top limit value of the last class interval must be greater than the largest value of the function you want to classify.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Because the channel contains the class limits, the number of channel values must be one value higher than the number of classes.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values you want to classify.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the class means.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the peak values 1.</td></tr>
<tr><td width="150">ClassMeth1</td>
<td>Specifies how DIAdem specifies the class limits.<div id="exp_ClassMeth1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginEnd"</pre></donottranslate></td>
<td>Number/Begin/End</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginWidth"</pre></donottranslate></td>
<td>Number/Begin/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginRange"</pre></donottranslate></td>
<td>Number/Begin/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"NoEndWidth"</pre></donottranslate></td>
<td>Number/End/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"NoEndRange"</pre></donottranslate></td>
<td>Number/End/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"BeginEndWidth"</pre></donottranslate></td>
<td>Begin/End/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"BeginWidthRange"</pre></donottranslate></td>
<td>Begin/Width/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"EndWidthRange"</pre></donottranslate></td>
<td>End/Width/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"Channel"</pre></donottranslate></td>
<td>Channel</td></tr>
</table>
</td></tr>
</table>
<p class="Body">When you use the <span class="Monospace">Automatic</span> method, you specify the number of classes. DIAdem calculates the missing parameters from the maximum and minimum values of the channel to be classified. If you use the <span class="Monospace">Channel</span> method, DIAdem uses the values of the specified channel as class limits.</p>
</div></td></tr>
<tr><td width="150">FrequencyType</td>
<td>Specifies whether DIAdem calculates the class frequency absolutely or relatively.<div id="exp_FrequencyType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"absolute"</pre></donottranslate></td>
<td>Absolute</td></tr>
<tr><td width="150"><donottranslate><pre>"relative"</pre></donottranslate></td>
<td>Relative</td></tr>
</table>
</td></tr>
</table>
<p class="Body">The <em>absolute class frequency</em> H<sub>i</sub> of the i-th class K<sub>i</sub> for i=1, 2, ...p for even numbers p of the created classes is equal the number of observation values in the class K<sub>i</sub>. The <em>relative class frequency</em> h<sub>i</sub> of the class K<sub>i</sub> is then <span class="Monospace">1/n</span> multiplied by the absolute class frequency.</p>
<p class="Body"><img border="0" height="39" src="image/v_fi_12.gif" width="60"/>with n = Channel length</p>
</div></td></tr>
<tr><td width="150">Hysteresis</td>
<td>Specifies the hysteresis as a percentage of the average class width.<div id="exp_Hysteresis">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= Hysteresis &lt;= 1000</td></tr>
</table>
<p class="Body">You can enter a hysteresis for classification methods that use one parameter and for the rainflow classification method in order to avoid slight fluctuations. DIAdem ignores an oscillation that occurs only within a class even if you do not set a hysteresis. Select the highest number of classes possible to keep the class width low.</p>
<p class="Body">If you select the channel method to define the class limits, the classes can have different widths. The hysteresis does not use the different class widths because DIAdem calculates the hysteresis as a percentage of the average class width.</p>
</div></td></tr>
<tr><td width="150">ClassRefLine</td>
<td>Specifies the zero line that divides the signal into positive and negative sections.<div id="exp_ClassRefLine">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">The zero line has the following meaning for the various classification methods:</p>
<table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" id="AutoNumber1" style="border-collapse: collapse">
<tr>
<td width="150">
<p class="Body" style="margin-top: 0pt; margin-bottom: 0pt">Peak value 1</p>
</td>
<td>
<p class="Body" style="margin-top: 0pt; margin-bottom: 0pt">DIAdem acquires only the largest peaks between two crossings of the zero line and registers these peaks in classes. DIAdem does not count the values before the first and after the last zero line crossing. Oscillation cycles where one extreme value is on the zero line, is only regarded as 'reference line crossed' if the other extreme value is below the reference line. If the zero line is at the class beginning, DIAdem does not count because there are no reference line crossings.</p>
</td>
</tr>
<tr>
<td width="150">
<p class="Body" style="margin-top: 0pt; margin-bottom: 0pt">Peak value 2</p>
</td>
<td>
<p class="Body" style="margin-top: 0pt; margin-bottom: 0pt">DIAdem acquires the maximum values above the zero line and the minimum values below the zero line. DIAdem considers a value that is on the zero line as a maximum value.</p>
</td>
</tr>
<tr>
<td width="150">
<p class="Body" style="margin-top: 0pt; margin-bottom: 0pt">Level crossing procedure</p>
</td>
<td>
<p class="Body" style="margin-top: 0pt; margin-bottom: 0pt">When a signal exceeds a class limit, DIAdem triggers a count. Below the zero line DIAdem only counts the negative slopes, above the zero line DIAdem only counts the positive slopes. If the zero line coincides with a class limit, DIAdem counts the positive slopes that exceed the zero line to the first positive class. DIAdem counts values that are on a class limit to the next higher class.</p>
</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[OpenBoundClass]</td>
<td>Specifies whether DIAdem counts values outside the class limits.<div id="exp_OpenBoundClass">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If this flag is set, DIAdem counts the values includes the values that are outside the class limits in the outer classes.</p>
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

*Source: `ComOff/ChnClassPeak1.htm`*
