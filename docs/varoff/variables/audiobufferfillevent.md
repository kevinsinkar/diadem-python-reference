---
title: "AudioBufferFillEvent"
description: "Specifies the user command that DIAdem calls when loading new data to the clipboard of the audio output."
---

# AudioBufferFillEvent

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: AudioBufferFillEvent

Specifies the user command that DIAdem calls when loading new data to the clipboard of the audio output.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>To prevent the audio output from slowing down, do not use commands in the user command that take a long time. Do not display message boxes or call other audio commands either.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AudioHandle</td>
<td>Specifies the handle of the audio output.</td></tr>
<tr><td width="150">CurrentIndex</td>
<td>Specifies which row of the channel DIAdem uses for filling the workspace.</td></tr>
<tr><td width="150">BlockSize</td>
<td>Specifies the number of values DIAdem uses for the buffer of the audio output.</td></tr>
<tr><td width="150">SampleRate</td>
<td>Specifies in Hz the sampling rate DIAdem uses to generate audio signals.</td></tr>
<tr><td width="150">MaxIndex</td>
<td>Specifies the maximum row index that corresponds to the minimum of both channel lengths.</td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def MyAudioOutCallback(AudioHandle, CurrentIndex, BlockSize, SampleRate, MaxIndex):
    # Some commands
```

---

*Source: `VarOff/AudioBufferFillEvent.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
