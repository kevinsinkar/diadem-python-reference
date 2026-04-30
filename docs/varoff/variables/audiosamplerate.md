---
title: "AudioSampleRate"
description: "Specifies in Hz the sampling rate DIAdem uses to generate audio signals. If you specify 0 or no value, DIAdem tries to specify the sampling rate from the proper"
---

# AudioSampleRate

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: AudioSampleRate

Specifies in Hz the sampling rate DIAdem uses to generate audio signals. If you specify 0 or no value, DIAdem tries to specify the sampling rate from the properties wf_xunit_string and wf_increment . If these properties are missing or in an incorrect unit, DIAdem uses the value 44.1 kHz.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Typical sampling rates are between 11 and 96 kHz. However not all sound boards support all sampling rates. Sound boards usually support at least the CD standard of 44.1 kHz.</td></tr></table>
</div>

---

*Source: `VarOff/AudioSampleRate.htm`*
