---
title: "ChnDRICalc"
description: "Calculates the Dynamic Response Index value (DRI). The Dynamic Response Index value is a criterion for axial compression force injuries to the thoracic-lumbar s"
---

# ChnDRICalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDRICalc

Calculates the Dynamic Response Index value (DRI). The Dynamic Response Index value is a criterion for axial compression force injuries to the thoracic-lumbar spine. The DRI is a dimensionless value related to the spine deflection.

## Signature

```python
return_value = dd.ChnDRICalc( XW , Y , ResultChannel , [DRIDirection], [DRIDampingCoefficient], [DRINaturalFrequency])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the signal in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration in  m/s^2.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>DIAdem generates a dimensionless result channel. The DRI value is the maximum value of this result channel.</td></tr>
<tr><td width="150">[DRIDirection]</td>
<td>Specifies the direction of the DRI calculation. If you do not set this parameter, DIAdem calculates the z-axis. <div id="exp_DRIDirection">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"X"</pre></donottranslate></td>
<td>X-axis</td></tr>
<tr><td width="150"><donottranslate><pre>"Y"</pre></donottranslate></td>
<td>Y-axis</td></tr>
<tr><td width="150"><donottranslate><pre>"Z"</pre></donottranslate></td>
<td>Z-axis</td></tr>
<tr><td width="150"><donottranslate><pre>"Free"</pre></donottranslate></td>
<td>Free</td></tr>
</table>
</td></tr>
</table>
<p>Depending on the selected axis, DIAdem uses the following damping coefficients and natural frequencies for the calculation: </p>
<table class="Borderless"><tr><td width="150">Damping coefficient for x-axis</td><td>0.2</td></tr><tr><td width="150">Damping coefficient for y-axis</td><td>0.09</td></tr><tr><td width="150">Damping coefficient for z-axis</td><td>0.224</td></tr><tr><td width="150">Natural frequency for x-axis</td><td>62.8 rad/s</td></tr><tr><td width="150">Natural frequency for y-axis</td><td>58.0 rad/s</td></tr><tr><td width="150">Natural frequency for z-axis</td><td>52.9 rad/s</td></tr></table>
<p class="Body">These values are from the following document: NASA/TM—2008-215198 (http://gltrs.grc.nasa.gov/reports/2008/TM-2008-215198.pdf)</p>
</div></td></tr>
<tr><td width="150">[DRIDampingCoefficient]</td>
<td>Specifies the damping coefficient if the DRI calculation is free.<div id="exp_DRIDampingCoefficient">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= DRIDampingCoefficient &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[DRINaturalFrequency]</td>
<td>Specifies the natural frequency of the dynamic system in rad/s if the DRI calculation is free.<div id="exp_DRINaturalFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= DRINaturalFrequency &lt;= 1E300</td></tr>
</table>
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

*Source: `ComOff/ChnDRICalc.htm`*
