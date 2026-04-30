---
title: "ChnHPCCalc"
description: "Calculates the Head Performance Criterion (HPC). The HPC value is a normalized maximum integral value of the head acceleration."
---

# ChnHPCCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnHPCCalc

Calculates the Head Performance Criterion (HPC). The HPC value is a normalized maximum integral value of the head acceleration.

## Signature

```python
dd.ChnHPCCalc( XW , Y , HPC36, HPC15, HPCVar, HPCUserDef, HPCUser)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem generally uses the resultant of the head acceleration in x, y and z-direction as the acceleration channel.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The input channels must be filtered with CFC1000.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">HPC criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the signal in seconds. The values of the data channel must be monotonic increasing. If the associated channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration values of the signal in gn (acceleration of gravity).</td></tr>
<tr><td width="150">HPC36</td>
<td>Specifies whether DIAdem calculates the 36 ms value.<div id="exp_HPC36">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HPC15</td>
<td>Specifies whether DIAdem calculates the 15 ms value.<div id="exp_HPC15">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HPCVar</td>
<td>Specifies whether DIAdem calculates the HPC value.<div id="exp_HPCVar">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HPCUserDef</td>
<td>Specifies whether DIAdem calculates the HPC value with adjustable window width.<div id="exp_HPCUserDef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">HPCUser</td>
<td>Specifies the width of the window in milliseconds when calculating the HPC value.<div id="exp_HPCUser">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= HPCUser &lt;= 1E10</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">HPCRes(i, j)</td><td>Receives the result matrix of the HPC calculation.<div id="exp_HPCRes">
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
<td width="150">HPCRes(1,1)</td>
<td width="150">Result<font face="Courier New" style="color: rgb(255, 0, 0);"><span class="style4"></span></font>~HPC~<span class="style2" style='font-family: "Courier New"; color: rgb(0, 0, 0);'></span>Value</td>
<td>Receives the HPC values for unlimited duration.</td></tr>
<tr>
<td width="150">HPCRes(2.1)</td>
<td width="150">Result~HPC~T1</td>
<td>Receives the T1 values for an unlimited duration.</td></tr>
<tr>
<td width="150">HPCRes(3.1)</td>
<td width="150">Result~HPC~T2</td>
<td>Receives the T2 values for an unlimited duration.</td></tr>
<tr>
<td width="150">HPCRes(4.1)</td>
<td width="150">Result~HPC~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for an unlimited duration.</td></tr>
<tr>
<td width="150">HPCRes(1.2)</td>
<td width="150">Result~HPC36~Value</td>
<td>Receives the HPC values for 36 ms.</td></tr>
<tr>
<td width="150">HPCRes(2.2)</td>
<td width="150">Result~HPC36~T1</td>
<td>Receives the T1 values for 36 ms.</td></tr>
<tr>
<td width="150">HPCRes(3.2)</td>
<td width="150">Result~HPC36~T2</td>
<td>Receives the T2 values for 36 ms.</td></tr>
<tr>
<td width="150">HPCRes(4.2)</td>
<td width="150">Result~HPC36~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for 36 ms.</td></tr>
<tr>
<td width="150">HPCRes(1.3)</td>
<td width="150">Result~HPC15~Value</td>
<td>Receives the HPC values for 15 ms.</td></tr>
<tr>
<td width="150">HPCRes(2.3)</td>
<td width="150">Result~HPC15~T1</td>
<td>Receives the T1 values for 15 ms.</td></tr>
<tr>
<td width="150">HPCRes(3.3)</td>
<td width="150">Result~HPC15~T2</td>
<td>Receives the T2 values for 15 ms.</td></tr>
<tr>
<td width="150">HPCRes(4.3)</td>
<td width="150">Result~HPC15~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for 15 ms.</td></tr>
<tr>
<td width="150">HPCRes(1.4)</td>
<td width="150">Result~HPCUser~Value</td>
<td>Receives the HPC values for the value specified in ms.</td></tr>
<tr>
<td width="150">HPCRes(2.4)</td>
<td width="150">Result~HPCUser~T1</td>
<td>Receives the T1 values for the value specified in ms.</td></tr>
<tr>
<td width="150">HPCRes(3.4)</td>
<td width="150">Result~HPCUser~T2</td>
<td>Receives the T2 values for the value specified in ms.</td></tr>
<tr>
<td width="150">HPCRes(4.4)</td>
<td width="150">Result~HPCUser~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for the value specified in ms.</td></tr>
<tr>
<td width="150">HPCRes(1.5)</td>
<td width="150">Result~HPCd~Value</td>
<td>Receives the HPC(d) values as an option.</td></tr>
<tr>
<td width="150">HPCRes(2.5)</td>
<td width="150">Result~HPCd~T1</td>
<td>Receives the T1 values of the HPC(d) calculation as an option.</td></tr>
<tr>
<td width="150">HPCRes(3.5)</td>
<td width="150">Result~HPCd~T1</td>
<td>Receives the T2 values of the HPC(d) calculation as an option.</td></tr>
<tr>
<td width="150">HPCRes(4.5)</td>
<td width="150">Result~HPCd~MeanAcceleration</td>
<td>Receives the mean value of the head acceleration between T1 and T2 for the HPC(d) calculation as an option.</td></tr>
<tr>
<td width="150"><a href="../../../varoff/variables/hcdversion/">HPCVersion</a></td>
<td width="150">Result~HPC~Version</td>
<td>Receives the algorithm version number, which is independent of the DIAdem version number.</td></tr>
<tr>
<td width="150">
   </td>
<td width="150">Result~HPCUser~WindowWidth</td>
<td>Receives the width of the window for calculating the HPC value in milliseconds.</td></tr>
</table>
</div></td></tr>
<tr><td width="150">HPCVersion</td><td>Receives the version number of the HPC calculation routine.<div id="exp_HPCVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnHPCCalc.htm`*
