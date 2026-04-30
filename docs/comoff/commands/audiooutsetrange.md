---
title: "AudioOutSetRange"
description: "Specifies the first and the last channel value of the audio output."
---

# AudioOutSetRange

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AudioOutSetRange

Specifies the first and the last channel value of the audio output.

## Signature

```python
dd.AudioOutSetRange(AudioHandle, AudioStartRow, AudioEndRow)
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
<tr><td width="150">AudioEndRow</td>
<td>Specifies the last channel row at which DIAdem ends the audio output. If you do not specify a value, if you specify a negative value, or if you specify a value larger than the channel length, DIAdem uses the last channel value.<div id="exp_AudioEndRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioEndRow &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/AudioOutSetRange.htm`*
