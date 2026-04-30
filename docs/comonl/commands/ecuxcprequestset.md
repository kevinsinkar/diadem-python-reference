---
title: "ECUXCPRequestSet"
description: "Performs a request to save session and device information to non-volatile memory."
---

# ECUXCPRequestSet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPRequestSet

Performs a request to save session and device information to non-volatile memory.

## Signature

```python
dd.ECUXCPRequestSet(ECUDeviceHandle, ECUMode, ECUXCPSessionID)
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
<tr><td width="150">ECUMode</td>
<td>Specifies a bit mask which describes the mode.<div id="exp_ECUMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUXCPSessionID</td>
<td>Specifies a configuration ID of the session in the non-volatile memory.<div id="exp_ECUXCPSessionID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUXCPSessionID &lt;= 65535</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPRequestSet.htm`*
