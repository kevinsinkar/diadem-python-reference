---
title: "ScaleMeasDeInit"
description: "Transfers the results of a calibration measurement to a scaling block."
---

# ScaleMeasDeInit

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ScaleMeasDeInit

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.DoubleVarSet('ScaleMeasPhys1', ...)   # instead of dd.ScaleMeasPhys1 = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Transfers the results of a calibration measurement to a scaling block.

## Signature

```python
dd.ScaleMeasDeInit(ScaleMeasBlName, ScaleMeasSigName)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table20">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/>
<br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call ScaleMeasDeInit(<em>BlockName</em>,<em>SignalName</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
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

*Source: `ComOnl/ScaleMeasDeInit.htm`*
