---
title: "ECUDatabaseOpen"
description: "Opens a specified A2L database."
---

# ECUDatabaseOpen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUDatabaseOpen

Opens a specified A2L database.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUDatabase</td>
<td>Specifies the path to an A2L database file which contains the description of the ECU. The file must use an A2L filename extension.<div id="exp_ECUDatabase">
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
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the handle for the database task. The return value is a ECUDatabasehandle type.<div id="exp_ECUDatabasehandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUDatabaseHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUDatabaseOpen.htm`*
