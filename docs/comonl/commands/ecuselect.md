---
title: "ECUSelect"
description: "Selects an ECU from an A2L database."
---

# ECUSelect

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUSelect

Selects an ECU from an A2L database.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUDatabasehandle</td>
<td>Specifies the handle for an A2L database.<div id="exp_ECUDatabasehandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUDatabaseHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUName</td>
<td>Specifies the name for accessing an element in an A2L database file. This name is, for example, the name of an ECU, a Characteristic, or a Measurement.<div id="exp_ECUName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUCommunicationProtocol</td>
<td>Specifies the communication logfile.<div id="exp_ECUCommunicationProtocol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ECUCommunicationProtocol &lt;= 2</td></tr>
</table>The <span class="Monospace">ECUCommunicationProtocol</span> variable can use the following constants:<table class="Borderless">
<tr>
<td>1</td>
<td width="150"><span class="Monospace">eECUCommunicationProtocolCCP</span></td>
<td>CCP (CAN Calibration Protocol)</td>
</tr>
<tr>
<td>2</td>
<td width="150"><span class="Monospace">eECUCommunicationProtocolXCP</span></td>
<td>XCP (Universal Measurement and Calibration Protocol)</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUCommunicationLayer</td>
<td>Specifies the communication layer.<div id="exp_ECUCommunicationLayer">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ECUCommunicationLayer &lt;= 6</td></tr>
</table>The <span class="Monospace">ECUCommunicationLayer</span> variable can use the following constants:<table class="Borderless">
<tr>
<td>1</td>
<td width="150"><span class="Monospace">eECUCommunicationLayerNIXNET</span></td>
<td>Communication through NI-XNET</td>
</tr>
<tr>
<td>2</td>
<td width="150"><span class="Monospace">eECUCommunicationLayerNICAN</span></td>
<td>Communication through NI-CAN</td>
</tr>
<tr>
<td>3</td>
<td width="150"><span class="Monospace">eECUCommunicationLayerTCP</span></td>
<td>Communication through TCP (if the variable <span class="Monospace">ECUCommunicationProtocol</span> has the value <span class="Monospace">eECUCommunicationProtocolXCP)</span></td>
</tr>
<tr>
<td>4</td>
<td width="150"><span class="Monospace">eECUCommunicationLayerUDP</span></td>
<td>Communication through UDP (if the variable <span class="Monospace">ECUCommunicationProtocol</span> has the value <span class="Monospace">eECUCommunicationProtocolXCP)</span></td>
</tr>
<tr>
<td>5</td>
<td width="150"><span class="Monospace">eECUCommunicationLayerVectorCAN</span></td>
<td>Communication through Vector XL Driver Library</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUCANInterface</td>
<td>Specifies which CAN interface to use (only for CCP and XCP on CAN).<div id="exp_ECUCANInterface">
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
<td>Contains the handle of the ECU. The return value is a ECUDeviceHandle type.<div id="exp_ECUDeviceHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUDeviceHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eECUCommunicationProtocolCCP` | 1 | CCP (CAN Calibration Protocol) |
| `eECUCommunicationProtocolXCP` | 2 | XCP (Universal Measurement and Calibration Protocol) |
| `eECUCommunicationLayerNIXNET` | 1 | Communication through NI-XNET |
| `eECUCommunicationLayerNICAN` | 2 | Communication through NI-CAN |
| `eECUCommunicationLayerTCP` | 3 | Communication through TCP (if the variable ECUCommunicationProtocol has the value eECUCommunicationProtocolXCP) |
| `eECUCommunicationLayerUDP` | 4 | Communication through UDP (if the variable ECUCommunicationProtocol has the value eECUCommunicationProtocolXCP) |
| `eECUCommunicationLayerVectorCAN` | 5 | Communication through Vector XL Driver Library |

---

*Source: `ComOnl/ECUSelect.htm`*
