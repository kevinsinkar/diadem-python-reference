---
title: "ChnRainCalc"
description: "Calculates the rainflow classification."
---

# ChnRainCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRainCalc

Calculates the rainflow classification.

## Signature

```python
dd.ChnRainCalc( Y , ClassMeth2, RainResiduumCalc, Hysteresis, RainFrequencyTyp)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To include all the values of a function in the classification, the bottom limit value of the first class interval must be smaller than the smallest value of the function you want to classify.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To include all the values of a function in the classification, the top limit value of the last class interval must be greater than the largest value of the function you want to classify.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You use the <a href="../../../varoff/variables/frequencypara/">FrequencyPara</a> variable to specify whether the rainflow classification calculates the cumulative frequency or the single frequency.</td>
</tr>
</table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You use the <a href="../../../varoff/variables/frequencypara/">FrequencyPara</a> variable to specify whether the rainflow classification calculates the cumulative frequency or the single frequency.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ClassMeth2</td>
<td>Specifies how DIAdem specifies the class limits.<div id="exp_ClassMeth2">
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
</table>
</td></tr>
</table>
<p class="Body">When you use the <span class="Monospace">Automatic</span> method, you specify the number of classes. DIAdem calculates the missing parameters from the maximum and minimum values of the channel to be classified.</p>
</div></td></tr>
<tr><td width="150">RainResiduumCalc</td>
<td>Specifies whether DIAdem includes the residues in the count.<div id="exp_RainResiduumCalc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
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
<tr><td width="150">RainFrequencyTyp</td>
<td>Specifies whether DIAdem displays the counts as a single frequency or as a cumulative frequency.<div id="exp_RainFrequencyTyp">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Cumulative"</pre></donottranslate></td>
<td>Accumulated frequency</td></tr>
<tr><td width="150"><donottranslate><pre>"Single"</pre></donottranslate></td>
<td>Single frequency</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnRainCalc.htm`*
