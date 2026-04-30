---
title: "CreateMQTT"
description: "Creates a MQTT object . The MQTT object provides the Message Queue Telemetry Transport Protocol in DIAdem. The MQTT protocol is an open message protocol for mac"
---

# CreateMQTT

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CreateMQTT

Creates a MQTT object . The MQTT object provides the Message Queue Telemetry Transport Protocol in DIAdem. The MQTT protocol is an open message protocol for machine-to-machine (M2M) communication for the transmission of telemetry data between devices. The communication of the individual devices between each other occurs over the MQTT broker. The MQTT broker is not an element of DIAdem.

## Signature

```python
return_value = dd.CreateMQTT(MqttUrl)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">MqttUrl</td>
<td>Specifies the URL of the MQTT broker. The URL can also contain the port. By default, DIAdem uses port <span class="Monospace">1883</span> for unencrypted communication and port <span class="Monospace">8883</span> for encrypted communication.<div id="exp_MqttUrl">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>An example for the URL is: "localhost" or "localhost:1883".</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">MQTT object</a> type.</td></tr>
</table>
</div>

## Python example

```python
def SFD_ReadChannel(ChannelNumberP, ParamP, DataP, ErrorP):
    MQTT  = dd.CreateMQTT(DeviceParam1V)
    sTemp = MQTT.ReadString(ParamP)

    if len(sTemp) == 0 :
        DataP = dd.NoValue
    else:
        if sTemp != "" :
            DataP = float(sTemp)
        else:
            DataP = dd.NoValue

def SFD_InitInChannel(ChannelNumberP, ParamP, ErrorP):
    MQTT.Subscribe(ParamP)

def SFD_Init(DeviceParam1V, DeviceParam2V, ErrorP):
    MQTT  = dd.CreateMQTT(DeviceParam1V)
    MQTT.Connect()
```

```python
def SFD_WriteChannel(ChannelNumberP, ParamP, DataP, ErrorP):
    MQTT.WriteString(ParamP, DataP)

def SFD_Init(DeviceParam1V, DeviceParam2V, ErrorP):
    MQTT  = dd.CreateMQTT(DeviceParam1V)
    MQTT.Connect
```

---

*Source: `ComOff/CreateMQTT.htm`*
