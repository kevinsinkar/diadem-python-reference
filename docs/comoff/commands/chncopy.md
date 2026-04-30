---
title: "ChnCopy"
description: "Copies a channel into another channel. You also can use the object-oriented interface to access internal data. Use Channels . AddChannels from the script interf"
---

# ChnCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCopy

Copies a channel into another channel. You also can use the object-oriented interface to access internal data. Use Channels . AddChannels from the script interface for internal data to realize the functionality of the ChnCopy command.

## Signature

```python
return_value = dd.ChnCopy( Y , ResultChannel , [ ChnXYRelation ])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the channel that DIAdem copies.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel. You only can copy channels of the same data type. If the target channel contains data, DIAdem overwrites the data. <span class="style1">If you create a new channel with <span class="Monospace">ChnCopy</span> and do not specify a name for the result channel, DIAdem assigns the name <span class="Monospace">Copy</span> to the result channel.</span></td></tr>
<tr><td width="150">[ChnXYRelation]</td>
<td>Specifies that x-channel references are used when copying and moving xy-channels and are preserved during reduced loading of xy-channels.<div id="exp_ChnXYRelation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Channel list variable</a> type. Receives the name of the result channel.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnCopy("Group1/SourceChannel","Group2/TargetChannel",True)
```

---

*Source: `ComOff/ChnCopy.htm`*
