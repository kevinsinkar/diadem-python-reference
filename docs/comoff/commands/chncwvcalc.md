---
title: "ChnCWVCalc"
description: "Calculates the chest wall velocity that occurs when the chest is crushed by a pressure wave. The chest wall velocity allows statements about injuries to interna"
---

# ChnCWVCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCWVCalc

Calculates the chest wall velocity that occurs when the chest is crushed by a pressure wave. The chest wall velocity allows statements about injuries to internal organs by overpressure waves which do not affect the ear.

## Signature

```python
return_value = dd.ChnCWVCalc( XW , Y , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="Image/note.gif" width="26"/></td><td><strong>Note  </strong>For further information such as mathematical background, input values, directives and rules, refer to the web site <a class="style1" href="https://www.sto.nato.int/publications/STO%20Technical%20Reports/RTO-TR-HFM-090/$$TR-HFM-090-ALL.pdf">RTO-TR-HFM-090 Test Methodology for Protection of Vehicle Occupants against Anti-Vehicular Landmine Effects</a> in paragraph 3.6.2.3 of the third chapter and in paragraph 1.2.2.2 of Appendix I.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the overpressure in Pascal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the values of the crest wall velocity in meters per second.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnCWVCalc.htm`*
