---
title: "ChnHICCalc"
description: "Calculates the Head Injury Criterion values (HIC). The HIC value is a normalized maximum integral value of the head acceleration."
---

# ChnHICCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnHICCalc

Calculates the Head Injury Criterion values (HIC). The HIC value is a normalized maximum integral value of the head acceleration.

## Signature

```python
dd.ChnHICCalc( XW , Y , HIC36, HIC15, HICVar, HICUserDef, HICUser, [HICd])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem generally uses the resultant of the head acceleration in x, y and z-direction as the acceleration channel.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">HIC criterion</a> for further information such as the mathematical background, input values, and directives and laws. </td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the signal in seconds. The values of the data channel must be monotonic increasing. If the associated channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration values of the signal in gn (acceleration of gravity).</td></tr>
<tr><td width="150">HIC36</td>
<td>Specifies whether DIAdem calculates the 36 ms value.<div id="exp_HIC36">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HIC15</td>
<td>Specifies whether DIAdem calculates the 15 ms value.<div id="exp_HIC15">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HICVar</td>
<td>Specifies whether DIAdem calculates the HIC value.<div id="exp_HICVar">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HICUserDef</td>
<td>Specifies whether DIAdem calculates the HIC value with adjustable window width.<div id="exp_HICUserDef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HICUser</td>
<td>Specifies the width of the window in milliseconds when calculating the HIC value.<div id="exp_HICUser">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= HICUser &lt;= 1E10</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[HICd]</td>
<td>Specifies whether DIAdem calculates the HIC(d) value. The default value is <span class="Monospace">FALSE</span> which means that DIAdem does not calculate the HIC(d) value.<div id="exp_HICd">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">HICRes(i, j)</td><td>Receives the result matrix of the HIC calculation.<div id="exp_HICRes">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a><br attr="ext"/>i = 1 ... <a href="../../../varoff/variables/hicresno/">HICResNo</a><br attr="ext"/>j = 1 ... <a href="../../../varoff/variables/hicrangeno/">HICRangeNo</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless">
<tr>
<td width="150"><strong>Result variable</strong></td>
<td width="150"><strong>Channel property</strong></td>
<td><strong>Description</strong></td></tr>
<tr>
<td width="150">HICRes(1.1)</td>
<td width="150">Result<font face="Courier New" style="color: rgb(255, 0, 0);"><span class="style4"></span></font>~HIC~<span class="style2" style='font-family: "Courier New"; color: rgb(0, 0, 0);'></span>Value</td>
<td>Receives the HIC values for unlimited duration.</td></tr>
<tr>
<td width="150">HICRes(2.1)</td>
<td width="150">Result~HIC~T1</td>
<td>Receives the T1 values for an unlimited duration.</td></tr>
<tr>
<td width="150">HICRes(3.1)</td>
<td width="150">Result~HIC~T2</td>
<td>Receives the T2 values for an unlimited duration.</td></tr>
<tr>
<td width="150">HICRes(4.1)</td>
<td width="150">Result~HIC~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for an unlimited duration.</td></tr>
<tr>
<td width="150">HICRes(1.2)</td>
<td width="150">Result~HIC36~Value</td>
<td>Receives the HIC values for 36 ms.</td></tr>
<tr>
<td width="150">HICRes(2.2)</td>
<td width="150">Result~HIC36~T1</td>
<td>Receives the T1 values for 36 ms.</td></tr>
<tr>
<td width="150">HICRes(3.2)</td>
<td width="150">Result~HIC36~T2</td>
<td>Receives the T2 values for 36 ms.</td></tr>
<tr>
<td width="150">HICRes(4.2)</td>
<td width="150">Result~HIC36~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for 36 ms.</td></tr>
<tr>
<td width="150">HICRes(1.3)</td>
<td width="150">Result~HIC15~Value</td>
<td>Receives the HIC values for 15 ms.</td></tr>
<tr>
<td width="150">HICRes(2.3)</td>
<td width="150">Result~HIC15~T1</td>
<td>Receives the T1 values for 15 ms.</td></tr>
<tr>
<td width="150">HICRes(3.3)</td>
<td width="150">Result~HIC15~T2</td>
<td>Receives the T2 values for 15 ms.</td></tr>
<tr>
<td width="150">HICRes(4.3)</td>
<td width="150">Result~HIC15~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for 15 ms.</td></tr>
<tr>
<td width="150">HICRes(1.4)</td>
<td width="150">Result~HICUser~Value</td>
<td>Receives the HIC values for the value specified in ms.</td></tr>
<tr>
<td width="150">HICRes(2.4)</td>
<td width="150">Result~HICUser~T1</td>
<td>Receives the T1 values for the value specified in ms.</td></tr>
<tr>
<td width="150">HICRes(3,4)</td>
<td width="150">Result~HICUser~T2</td>
<td>Receives the T2 values for the value specified in ms.</td></tr>
<tr>
<td width="150">HICRes(4.4)</td>
<td width="150">Result~HICUser~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for the value specified in ms.</td></tr>
<tr>
<td width="150">HICRes(1.5)</td>
<td width="150">Result~HICd~Value</td>
<td>Receives the HIC(d) values.</td></tr>
<tr>
<td width="150">HICRes(2.5)</td>
<td width="150">Result~HICd~T1</td>
<td>Receives the T1 values for the HIC(d) calculation.</td></tr>
<tr>
<td width="150">HICRes(3.5)</td>
<td width="150">Result~HICd~T1</td>
<td>Receives the T2 values for the HIC(d) calculation.</td></tr>
<tr>
<td width="150">HICRes(4.5)</td>
<td width="150">Result~HICd~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for the HIC(d) calculation.</td></tr>
<tr>
<td width="150"><a href="../../../varoff/variables/hicversion/">HICVersion</a></td>
<td width="150">Result~HIC~Version</td>
<td>Receives the algorithm version number, which is independent of the DIAdem version number.</td></tr>
<tr>
<td width="150">
   </td>
<td width="150">Result~HICUser~WindowWidth</td>
<td>Receives the width of the window for calculating the HIC value in milliseconds.</td></tr>
</table>
</div></td></tr>
<tr><td width="150">HICVersion</td><td>Receives the version number of the HIC calculation routine.<div id="exp_HICVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnHICCalc.htm`*
