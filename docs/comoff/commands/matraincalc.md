---
title: "MatRainCalc"
description: "Evaluates a rainflow or transition matrix."
---

# MatRainCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatRainCalc

Evaluates a rainflow or transition matrix.

## Signature

```python
dd.MatRainCalc( X , Y , Z , RainFrequencyTyp)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>Z</em></td>
<td>Specifies the data channel containing the z-values.</td></tr>
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

*Source: `ComOff/MatRainCalc.htm`*
