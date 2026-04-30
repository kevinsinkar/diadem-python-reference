---
title: "ChnKTHCalc"
description: "Calculates the Knee Thigh Hip (KTH) value, which represents the risk of injury to the hip and thigh."
---

# ChnKTHCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnKTHCalc

Calculates the Knee Thigh Hip (KTH) value, which represents the risk of injury to the hip and thigh.

## Signature

```python
dd.ChnKTHCalc( XW , Y )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  DIAdem saves the calculation results and the version number of the algorithm which is not the same as the DIAdem version number in the following custom properties of the result channel: <span class="Monospace">Result~KTH~Rating</span>, <span class="Monospace">Result~KTH~FMax</span>, <span class="Monospace">Result~KTH~t0</span>, <span class="Monospace">Result~KTH~t1</span>, and <span class="Monospace">Result~KTH~Version</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the signal in milliseconds. If the associated channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the forces in Newton.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">KTHRating</td><td>Receives the evaluation of the KTH calculation through the maximum value and the impulse.<div id="exp_KTHRating">
<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Enumeration variable</a> with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Good"</pre></donottranslate></td>
<td>Good</td></tr>
<tr><td width="150"><donottranslate><pre>"Acceptable"</pre></donottranslate></td>
<td>Acceptable</td></tr>
<tr><td width="150"><donottranslate><pre>"Marginal"</pre></donottranslate></td>
<td>Marginal</td></tr>
<tr><td width="150"><donottranslate><pre>"Poor"</pre></donottranslate></td>
<td>Poor</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">KTHFmax</td><td>Receives the maximum value of the forces impacting the hips and thighs, in kilo newton.<div id="exp_KTHFmax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0.0 &lt;= KTHFMax &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">KTHImpuls</td><td>Receives the impulse of KTHt0 after KTHt1, in Newton seconds.<div id="exp_KTHImpulse">
<table class="Borderless">
<tr><td style="height: 21px"><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0.0 &lt;= KTHImpulse &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">KTHt0</td><td>Receives the time span until the last zero crossing before reaching the maximum value, in milliseconds.<div id="exp_KTHt0">
<table class="Borderless">
<tr><td style="height: 21px"><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0.0 &lt;= KTHt0 &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">KTHt1</td><td>Receives the time span as far as the falling slope after reaching the maximum value, in milliseconds.<div id="exp_KTHt1">
<table class="Borderless">
<tr><td style="height: 21px"><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>0.0 &lt;= KTHt1 &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">KTHVersion</td><td>Receives the version number of the KTH calculation routine.<div id="exp_KTHVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr><td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ChnKTHCalc("[1]/Time", "[1]/Data")
dd.MsgBoxDisp ("KTHRating = " + dd.KTHRating+ "\r\n" + "KTH version: " + dd.KTHVersion)
```

---

*Source: `ComOff/ChnKTHCalc.htm`*
