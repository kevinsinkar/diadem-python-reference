---
title: "ChnXGCalc"
description: "Determines the total time in milliseconds for which the acceleration signal is x-times gn (gravity acceleration)."
---

# ChnXGCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnXGCalc

Determines the total time in milliseconds for which the acceleration signal is x-times gn (gravity acceleration).

## Signature

```python
dd.ChnXGCalc( XW , Y , XGRes, XGType)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the input channel: <span class="Monospace">ResultXgDeltaX</span>, <span class="Monospace">ResultXgMaxPeak</span>, <span class="Monospace">ResultXgTimeBegin</span>, <span class="Monospace">ResultXgTimeEnd</span>, and <span class="Monospace">ResultXgVersion</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">Xg criterion</a> for further information such as background, input value, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150">XGRes</td>
<td>Specifies the acceleration in gn (gravity acceleration).<div id="exp_XGRes">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XGType</td>
<td>Specifies whether DIAdem calculates the acceleration, which lasts X ms, from one section or several partial sections.<div id="exp_XGType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"in one peak"</pre></donottranslate></td>
<td>In one peak</td></tr>
<tr><td width="150"><donottranslate><pre>"in multiple peaks"</pre></donottranslate></td>
<td>In multiple peaks</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">XgTimeBegin</td><td>Receives the time T1 of the calculated Xg acceleration in milliseconds.<div id="exp_XgTimeBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XgTimeEnd</td><td>Receives the time T2 of the calculated Xg acceleration in milliseconds.<div id="exp_XgTimeEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XgMaxPeak</td><td>Receives the time interval between T1 and T2 for the Xg calculation in milliseconds.<div id="exp_XgMaxPeak">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XgDeltaX</td><td>Receives the total time of the Xg calculation for several sections in milliseconds.<div id="exp_XgDeltaX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XgVersion</td><td>Receives the version number of the Xg calculation routine.<div id="exp_XgVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnXGCalc.htm`*
