---
title: "ChnHCDCalc"
description: "Calculates the Head Contact Duration values (HCD). The HCD value is a normalized maximum integral value of the head acceleration."
---

# ChnHCDCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnHCDCalc

Calculates the Head Contact Duration values (HCD). The HCD value is a normalized maximum integral value of the head acceleration.

## Signature

```python
dd.ChnHCDCalc( XW , Y , Y1 , HCD36, HCD15, HCDVar, HCDUserDef, HCDUser)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem generally uses the resultant of the head acceleration in x, y and z-direction as the acceleration channel.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">HCD criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds. The values of the data channel must be monotonic increasing. If the associated channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration values of the signal in gn (acceleration of gravity).</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the resulting neck forces in Newton.</td></tr>
<tr><td width="150">HCD36</td>
<td>Specifies whether DIAdem calculates the 36 ms value.<div id="exp_HCD36">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HCD15</td>
<td>Specifies whether DIAdem calculates the 15 ms value.<div id="exp_HCD15">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HCDVar</td>
<td>Specifies whether DIAdem calculates the HCD value.<div id="exp_HCDVar">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HCDUserDef</td>
<td>Specifies whether DIAdem calculates the HCD value with adjustable window width.<div id="exp_HCDUserDef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HCDUser</td>
<td>Specifies the width of the window in milliseconds when calculating the HCD value.<div id="exp_HCDUser">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= HCDUser &lt;= 1E10</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">HCDRes(i, j)</td><td>Receives the result matrix of the HCD calculation.<div id="exp_HCDRes">
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
<td width="150">HCDRes(1,1)</td>
<td width="150">Result<font face="Courier New" style="color: rgb(255, 0, 0);"><span class="style4"></span></font>~HPC~<span class="style2" style='font-family: "Courier New"; color: rgb(0, 0, 0);'></span>Value</td>
<td>Receives the HCD values for unlimited duration.</td></tr>
<tr>
<td width="150">HCDRes(2.1)</td>
<td width="150">Result~HCD~T1</td>
<td>Receives the T1 values for an unlimited duration.</td></tr>
<tr>
<td width="150">HCDRes(3.1)</td>
<td width="150">Result~HCD~T2</td>
<td>Receives the T2 values for an unlimited duration.</td></tr>
<tr>
<td width="150">HCDRes(4.1)</td>
<td width="150">Result~HCD~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for an unlimited duration.</td></tr>
<tr>
<td width="150">HCDRes(1.2)</td>
<td width="150">Result~HCD36~Value</td>
<td>Receives the HCD values for 36 ms.</td></tr>
<tr>
<td width="150">HCDRes(2.2)</td>
<td width="150">Result~HCD36~T1</td>
<td>Receives the T1 values for 36 ms.</td></tr>
<tr>
<td width="150">HCDRes(3.2)</td>
<td width="150">Result~HCD36~T2</td>
<td>Receives the T2 values for 36 ms.</td></tr>
<tr>
<td width="150">HCDRes(4.2)</td>
<td width="150">Result~HCD36~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for 36 ms.</td></tr>
<tr>
<td width="150">HCDRes(1.3)</td>
<td width="150">Result~HCD15~Value</td>
<td>Receives the HCD values for 15 ms.</td></tr>
<tr>
<td width="150">HCDRes(2.3)</td>
<td width="150">Result~HCD15~T1</td>
<td>Receives the T1 values for 15 ms.</td></tr>
<tr>
<td width="150">HCDRes(3.3)</td>
<td width="150">Result~HCD15~T2</td>
<td>Receives the T2 values for 15 ms.</td></tr>
<tr>
<td width="150">HCDRes(4.3)</td>
<td width="150">Result~HCD15~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for 15 ms.</td></tr>
<tr>
<td width="150">HCDRes(1.4)</td>
<td width="150">Result~HCDd~Value</td>
<td>Receives the HCD values for the value specified in ms.</td></tr>
<tr>
<td width="150">HCDRes(2.4)</td>
<td width="150">Result~HCDd~T1</td>
<td>Receives the T1 values for the value specified in ms.</td></tr>
<tr>
<td width="150">HCDRes(3.4)</td>
<td width="150">Result~HCDd~T1</td>
<td>Receives the T2 values for the value specified in ms.</td></tr>
<tr>
<td width="150">HCDRes(4.4)</td>
<td width="150">Result~HCDd~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for the value specified in ms.</td></tr>
<tr>
<td width="150"><a href="../../../varoff/variables/hcdversion/">HCDVersion</a></td>
<td width="150">Result~HCD~Version</td>
<td>Receives the algorithm version number, which is independent of the DIAdem version number.</td></tr>
<tr>
<td width="150">
   </td>
<td width="150">Result~HCDUser~WindowWidth</td>
<td>Receives the width of the window for calculating the HCD value in milliseconds.</td></tr>
</table>
</div></td></tr>
<tr><td width="150">HCDVersion</td><td>Receives the version number of the HCD calculation routine.<div id="exp_HCDVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnHCDCalc.htm`*
