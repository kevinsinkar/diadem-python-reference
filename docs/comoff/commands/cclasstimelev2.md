---
title: "CClassTimeLev2"
description: "Calculates the compound classification with the time-at-level counting method II."
---

# CClassTimeLev2

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CClassTimeLev2

Calculates the compound classification with the time-at-level counting method II.

## Signature

```python
dd.CClassTimeLev2( Y , Y1 , X , ClassMeth2, FrequencyType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem saves the result matrix in the default group.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel of the first signal.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel of the second signal.</td></tr>
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the joint x-values.</td></tr>
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
</table>
</div>

---

*Source: `ComOff/CClassTimeLev2.htm`*
