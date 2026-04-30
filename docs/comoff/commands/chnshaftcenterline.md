---
title: "ChnShaftCenterline"
description: "Calculates the movement of a rotating shaft over an extended time period. The measurement values of two sensors at the shaft are averaged in order to specify ho"
---

# ChnShaftCenterline

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnShaftCenterline

Calculates the movement of a rotating shaft over an extended time period. The measurement values of two sensors at the shaft are averaged in order to specify how the position of the shaft center changes over several revolutions.

## Signature

```python
return_value = dd.ChnShaftCenterline( ShaftCenterlineInputX , ShaftCenterlineInputY , ResultChannel , ResultChannel , ShaftCenterlineGapRefX, ShaftCenterlineGapRefY, ShaftCenterlineIntervalType, ShaftCenterlineNoOfIntervals, ShaftCenterlineIntervalLength)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The command processes input channels even if these contain NoValues.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ShaftCenterlineInputX</td>
<td>Specifies one or more channels with x-values of the measured orbit rotations.<div id="exp_ShaftCenterlineInputX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ShaftCenterlineInputY</td>
<td>Specifies one or more channels with y-values of the measured orbit rotations.<div id="exp_ShaftCenterlineInputY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies one or more channels with x-values of the measured orbit rotations.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies one or more channels with y-values of the measured orbit rotations.</td></tr>
<tr><td width="150">ShaftCenterlineGapRefX</td>
<td>Specifies the x-margin to the shaft centerline.<div id="exp_ShaftCenterlineGapRefX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ShaftCenterlineGapRefY</td>
<td>Specifies the y-margin to the shaft centerline.<div id="exp_ShaftCenterlineGapRefY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ShaftCenterlineIntervalType</td>
<td>Specifies the data amount for the calculation.<div id="exp_ShaftCenterlineIntervalType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NoOfIntervals"</pre></donottranslate></td>
<td>Number of intervals</td></tr>
<tr><td width="150"><donottranslate><pre>"IntervalLength"</pre></donottranslate></td>
<td>Length of the intervals</td></tr>
<tr><td width="150"><donottranslate><pre>"All"</pre></donottranslate></td>
<td>All</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ShaftCenterlineNoOfIntervals</td>
<td>Specifies the number of intervals.<div id="exp_ShaftCenterlineNoOfIntervals">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ShaftCenterlineNoOfIntervals &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ShaftCenterlineIntervalLength</td>
<td>Specifies the number of values in an interval.<div id="exp_ShaftCenterlineIntervalLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ShaftCenterlineIntervalLength &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnShaftCenterline.htm`*
