---
title: "ScaleMeasInit"
description: "Reads the parameters for a calibration measurement."
---

# ScaleMeasInit

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ScaleMeasInit

Reads the parameters for a calibration measurement.

## Signature

```python
dd.ScaleMeasInit(ScaleMeasBlName, ScaleMeasSigName)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table24">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/>
<br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)
    Call ScaleMeasInit(<em>BlockName</em>,<em>SignalName</em>)
Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
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

## Python example

```python
dd.DACObjOpen("2Point")
dd.ScaleMeasInit("2Point","Temp1")
dd.ScaleMeasVal1Get("2Point","Temp1")
dd.ScaleMeasVal2Get("2Point","Temp1")
dd.ScaleMeasDeInit("2Point","Temp1")
dd.DACObjClose("2Point")
```

---

*Source: `ComOnl/ScaleMeasInit.htm`*
