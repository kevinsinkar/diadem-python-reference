---
title: "ConvertTimeType"
description: "Converts a time data type to another time data type."
---

# ConvertTimeType

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ConvertTimeType

Converts a time data type to another time data type.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SourceDateTime</td>
<td>Specifies the time to convert. DIAdem automatically specifies the data type of the time to be converted. It can be the same data type as one of the data types specified in <span class="Monospace">TargetType</span>. Use the <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a> variable to resolve DIAdem time data.<div id="exp_SourceDateTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">TargetType</td>
<td>Specifies the data type of the returned time value.<div id="exp_TargetType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= TargetType &lt;= 3</td></tr>
</table>
<table class="Borderless">
<tr>
<td>The following selection terms are available<table class="Borderless">
<tr>
<td width="150"><strong>Script Term</strong></td>
<td width="50"><strong>Value</strong></td>
<td><strong>Interface Term, Explanation</strong></td>
</tr>
<tr>
<td width="150"><donottranslate>
<pre>eConvertvbDateTime</pre>
</donottranslate></td>
<td width="50">0</td>
<td>VBScript variant with subtype <a href="#" data-unresolved="1">vbDate</a>.</td>
</tr>
<tr>
<td width="150"><donottranslate>
<pre>eConvertDIAdemDateTime </pre>
</donottranslate></td>
<td width="50">1</td>
<td>Double value in DIAdem time format. Use the <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a> variable to resolve DIAdem time data.</td>
</tr>
<tr>
<td width="150"><donottranslate>
<pre>eConvertStringDateTime </pre>
</donottranslate></td>
<td width="50">2</td>
<td>Text in a time format that correspond to the standard time format specified in <strong>Settings»DIAdem Settings»General</strong>. DIAdem saves the default time format in the variable <a href="../../../varoff/variables/timeformat/">TimeFormat</a>.</td>
</tr>
<tr>
<td width="150"><donottranslate>
<pre>eConvertUSITimeDisp </pre>
</donottranslate></td>
<td width="50">3</td>
<td><a href="../../../scriptnavi/objects/itdmtimedisp/">USITimeDisp-Object</a> with date/time information.</td>
</tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant variable</a> type. The data type corresponds to the data type specified in <span class="Monospace">TargetType</span>.</td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eConvertvbDateTime` | 0 | VBScript variant with subtype vbDate . |
| `eConvertDIAdemDateTime` | 1 | Double value in DIAdem time format. Use the ApplicationTimebaseHighResolution variable to resolve DIAdem time data. |
| `eConvertStringDateTime` | 2 | Text in a time format that correspond to the standard time format specified in Settings»DIAdem Settings»General . DIAdem saves the default time format in the variable TimeFormat . |
| `eConvertUSITimeDisp` | 3 | USITimeDisp-Object with date/time information. |

## Python example

```python
Range = "week"
oStartTime = dd.CreateTime(1999,11,20,0,0,0)
dStartTime = dd.ConvertTimeType (oStartTime,dd.eConvertDIAdemDateTime )
dd.ChnGenTime ("[]/GenTimeChn_dTime", Range, dStartTime, 0, 1, "StartStepNo", 10)
```

---

*Source: `ComOff/ConvertTimeType.htm`*
