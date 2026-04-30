---
title: "ScaleMeasVal2Get"
description: "Determines the second value of the input range of a calibration measurement."
---

# ScaleMeasVal2Get

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ScaleMeasVal2Get

Determines the second value of the input range of a calibration measurement.

## Signature

```python
dd.ScaleMeasVal2Get(ScaleMeasBlName, ScaleMeasSigName)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table30">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call ScaleMeasVal1Get(<em>BlockName</em>,<em>SignalName</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ScaleMeasBlName</td>
<td>Specifies the name of a DAC block that DIAdem uses to run a calibration.<div id="exp_ScaleMeasBlName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ScaleMeasSigName</td>
<td>Specifies the name of the signal that DIAdem uses to run a calibration.<div id="exp_ScaleMeasSigName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table26">
<tr>
<td width="150">ScaleMeasInp2</td>
<td>Receives the first value of the input range of a calibration measurement. In the calibration measurement DIAdem converts this value into the first value of the physical quantity.<div id="exp_ScaleMeasInp2">
<table class="Borderless" id="table27">
<tr>
<td><a href="#" data-unresolved="1">Floating-point number variable</a></td>
</tr>
<tr>
<td>-1E36 &lt;= ScaleMeasInp2 &lt;= +1E36</td>
</tr>
</table>
</div>
</td>
</tr>
</table>
</div>

## Python example

```python
dd.DACObjOpen("2Point")
dd.ScaleMeasInit("2Point","Temp1")
dd.ScaleMeasVal1Get("2Point","Temp1")
dd.ScaleMeasVal2Get("2Point","Temp1")
dd.ScaleMeasDeInit("2Point","Temp1")
dd.DACObjClose("2Point")
```

```python
dd.ScaleMeasPhys1= 0
dd.ScaleMeasPhys2= 1234
dd.ScaleMeasDim= "[---]"
dd.DACObjOpen("2Point")
dd.ScaleMeasVal1Get("2Point","Temp1")
dd.ScaleMeasVal2Get("2Point","Temp1")
dd.ScaleMeasDeInit("2Point","Temp1")
dd.DACObjClose("2Point")
```

---

*Source: `ComOnl/ScaleMeasVal2Get.htm`*
