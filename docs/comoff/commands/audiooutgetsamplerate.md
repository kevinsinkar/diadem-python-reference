---
title: "AudioOutGetSampleRate"
description: "Receives the sampling rate of the audio output."
---

# AudioOutGetSampleRate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AudioOutGetSampleRate

Receives the sampling rate of the audio output.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Typical sampling rates are between 11 and 96 kHz. However not all sound boards support all sampling rates. Sound boards usually support at least the CD standard of 44.1 kHz.</td></tr></table>
</div>

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
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies in Hz the sampling rate DIAdem uses to generate audio signals. If you specify <span class="Monospace">0</span> or no value, DIAdem tries to specify the sampling rate from the properties <span class="Monospace">wf_xunit_string</span> and <span class="Monospace">wf_increment</span>. If these properties are missing or in an incorrect unit, DIAdem uses the value 44.1 kHz. The return value is a AudioSampleRate type.<div id="exp_AudioSampleRate">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioSampleRate &lt;= 96000</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Typical sampling rates are between 11 and 96 kHz. However not all sound boards support all sampling rates. Sound boards usually support at least the CD standard of 44.1 kHz.</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/AudioOutGetSampleRate.htm`*
