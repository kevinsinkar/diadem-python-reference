---
title: "ChnQuantize"
description: "Maps the values of a channel in quantization steps."
---

# ChnQuantize

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnQuantize

Maps the values of a channel in quantization steps.

## Signature

```python
return_value = dd.ChnQuantize( Y , ResultChannel , QuantResolution, QuantRangeMin, QuantRangeMax)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For further information such as mathematical background, input values, directives and rules, refer to the web site <a class="style1" href="https://www.sto.nato.int/publications/STO%20Technical%20Reports/RTO-TR-HFM-090/$$TR-HFM-090-ALL.pdf">RTO-TR-HFM-090 Test Methodology for Protection of Vehicle Occupants against Anti-Vehicular Landmine Effects</a> in paragraph 3.6.2.3 of the third chapter and in paragraph 1.2.2.2 of Appendix I.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values to be processed.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">QuantResolution</td>
<td>Specifies the number of steps into which DIAdem divides a channel.<div id="exp_QuantResolution">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>2 &lt;= QuantResolution &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">QuantRangeMin</td>
<td>Specifies the bottom range limit where DIAdem starts dividing a channel.<div id="exp_QuantRangeMin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table> To optimally adjust the channel to the range, use the channel minimum as the upper range limit: <span class="Monospace">Data.Root.ChannelGroups(<em>ChannelGroup</em>).Channels(<em>Channel</em>).Properties("minimum").<a href="../../../inavidata/properties/idiademproperty-value/">Value</a></span></div></td></tr>
<tr><td width="150">QuantRangeMax</td>
<td>Specifies the top range limit up to which DIAdem divides a channel.<div id="exp_QuantRangeMax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table> To optimally adjust the channel to the range, use the channel maximum as the upper range limit: <span class="Monospace">Data.Root.ChannelGroups(<em>ChannelGroup</em>).Channels(<em>Channel</em>).Properties("maximum").<a href="../../../inavidata/properties/idiademproperty-value/">Value</a></span></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnQuantize.htm`*
