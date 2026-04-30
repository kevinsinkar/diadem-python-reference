---
title: "ECUXCPCalibPageCopy"
description: "Forces a copy operation from one calibration page to another calibration page."
---

# ECUXCPCalibPageCopy

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPCalibPageCopy

Forces a copy operation from one calibration page to another calibration page.

## Signature

```python
dd.ECUXCPCalibPageCopy(ECUDeviceHandle, ECUSourceSegment, ECUSourcePage, ECUTargetSegment, ECUTargetPage)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUDeviceHandle</td>
<td>Specifies the handle for the ECU.<div id="exp_ECUDeviceHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUDeviceHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUSourceSegment</td>
<td>Specifies the logical number of the source data segment.<div id="exp_ECUSourceSegment">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUSourcePage</td>
<td>Specifies the logical number of the source page.<div id="exp_ECUSourcePage">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUTargetSegment</td>
<td>Specifies the logical number of the source destination data segment.<div id="exp_ECUTargetSegment">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUTargetPage</td>
<td>Specifies the logical number of the destination page.<div id="exp_ECUTargetPage">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPCalibPageCopy.htm`*
