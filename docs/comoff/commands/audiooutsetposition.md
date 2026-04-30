---
title: "AudioOutSetPosition"
description: "Specifies the position of the audio output in the specified play range."
---

# AudioOutSetPosition

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AudioOutSetPosition

Specifies the position of the audio output in the specified play range.

## Signature

```python
dd.AudioOutSetPosition(AudioHandle, AudioStartRow)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AudioHandle</td>
<td>Specifies the handle of the audio output.<div id="exp_AudioHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-2147483648 &lt;= AudioHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AudioStartRow</td>
<td>Specifies the first channel row from where DIAdem starts the audio output. If you do not specify a value or if you specify a negative value, DIAdem uses the first value of the channel.<div id="exp_AudioStartRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioStartRow &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/AudioOutSetPosition.htm`*
