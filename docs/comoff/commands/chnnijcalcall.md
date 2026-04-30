---
title: "ChnNijCalcAll"
description: "Simultaneously calculates the Normalized Neck Injury Criterion value (Nij) according to FMVSS for all four calculation types (NTE, NTF, NCE and NCF)."
---

# ChnNijCalcAll

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNijCalcAll

Simultaneously calculates the Normalized Neck Injury Criterion value (Nij) according to FMVSS for all four calculation types (NTE, NTF, NCE and NCF).

## Signature

```python
return_value = dd.ChnNijCalcAll( XW , Y , Y1 , NijMaxFlexion, NijMaxExtension, NijMaxTension, NijMaxCompression, NijNormalizedOutput)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem saves the calculation results and the version number of the algorithm use in the following custom properties of the result channel: <span class="Monospace">Result~Nij~Max</span>, <span class="Monospace">Result~Nij~Time</span>, and <span class="Monospace">Result~Nij~Version</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">NIJ criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in milliseconds. The values of the data channel must be monotonic increasing. If the y-channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values of the axial force in the z-direction at the point where the head intersects with the neck, in Newton.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the y1-values.</td></tr>
<tr><td width="150">NijMaxFlexion</td>
<td>Specifies the critical compression force in newtons in the positive z-direction.<div id="exp_NijMaxFlexion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= NijMaxFlexion &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">NijMaxExtension</td>
<td>Specifies the critical bending moment in newton meters in the positive y-direction.<div id="exp_NijMaxExtension">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>-1E300 &lt;= NijMaxExtension &lt;= 0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">NijMaxTension</td>
<td>Specifies the critical tensile force in newtons in the negative z-direction.<div id="exp_NijMaxTension">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= NijMaxTension &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">NijMaxCompression</td>
<td>Specifies the critical bending moment in newton meters in the negative y-direction.<div id="exp_NijMaxCompression">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>-1E300 &lt;= NijMaxCompression &lt;= 0<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">NijNormalizedOutput</td>
<td>Specifies whether DIAdem normalizes the result values ranging from -1 to +1.<div id="exp_NijNormalizedOutput">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
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

*Source: `ComOff/ChnNijCalcAll.htm`*
