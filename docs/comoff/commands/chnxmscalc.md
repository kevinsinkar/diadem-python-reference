---
title: "ChnXMSCalc"
description: "Determines the maximum acceleration value that lasts at least x milliseconds."
---

# ChnXMSCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnXMSCalc

Determines the maximum acceleration value that lasts at least x milliseconds.

## Signature

```python
dd.ChnXMSCalc( XW , Y , XMSRes, [XMSTolerance], [XMSType], [XMSNegSigValCalc])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the input channel:  <span class="Monospace">ResultXmsAcceleration</span>, <span class="Monospace">ResultXmsTimeBegin</span>, <span class="Monospace">ResultXmsTimeEnd</span>, <span class="Monospace">ResultXmsDeltaX</span>, and <span class="Monospace">ResultXmsVersion</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the <span class="Monospace">XMSNegSigNalCalc</span> variable has the value <span class="Monospace">TRUE</span>, DIAdem calculates the X ms values for the positive signal section and separately from the absolute value for the negative signal section. DIAdem sets the value for the other signal section to zero. DIAdem saves the X ms values of the higher absolute acceleration in the result variables.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong><span class="Monospace">3</span> is a typical setting for the <span class="Monospace">XMSRes</span> variable.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">Xms criterion</a> for further information such as background, input value, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150">XMSRes</td>
<td>Specifies the time X in milliseconds.<div id="exp_XMSRes">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= XmsRes &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[XMSTolerance]</td>
<td>For future extensions.</td></tr>
<tr><td width="150">[XMSType]</td>
<td>Specifies whether DIAdem calculates the acceleration from one section or several sections. The default value of the <span class="Monospace">XMSType</span> variable is <span class="Monospace">in one peak</span>.<div id="exp_XMSType">
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
<tr><td width="150">[XMSNegSigValCalc]</td>
<td>Specifies whether DIAdem includes the negative signal sections in the X ms calculation. The default value is <span class="Monospace">FALSE</span> which specifies that DIAdem does not consider the negative signal parts.<div id="exp_XMSNegSigValCalc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If the <span class="Monospace">XmsNegSigValCalc</span> variable has the value <span class="Monospace">TRUE</span>, DIAdem calculates the X ms values for the positive signal section separately from the absolute value for the negative signal section. DIAdem sets the value for the other signal section to zero. DIAdem saves the X ms values of the higher absolute acceleration in the result variables.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">XmsAcceleration</td><td>Receives the acceleration of the X ms calculation.<div id="exp_XmsAcceleration">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XmsTimeBegin</td><td>Receives the time T1 of the calculated X ms acceleration in milliseconds.<div id="exp_XmsTimeBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XmsTimeEnd</td><td>Receives the time T2 of the calculated X ms acceleration in milliseconds.<div id="exp_XmsTimeEnd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XmsDeltaX</td><td>Receives the determined time T of the X ms calculation in milliseconds.<div id="exp_XmsDeltaX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">XmsVersion</td><td>Receives the version number of the X ms calculation routine.<div id="exp_XmsVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnXMSCalc.htm`*
