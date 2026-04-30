---
title: "ChnTTICalc"
description: "Calculates the Thorax Trauma Index (TTI). This value is the injury criterion for the chest area."
---

# ChnTTICalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnTTICalc

Calculates the Thorax Trauma Index (TTI). This value is the injury criterion for the chest area.

## Signature

```python
dd.ChnTTICalc( XW , Y , Y1 , Y2 , [FIR100SampleType])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem saves the results and the algorithm version number, which does not depend on the DIAdem version number, in the following custom properties: <span class="Monospace">Result~TTI~Result</span> and <span class="Monospace">Result~TTI~Version</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Before the calculation, DIAdem filters the input channels with the FIR100 filter.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">TTI criterion</a> for further information such as background, input value, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the unfiltered acceleration values of the lower rib in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel that contains the unfiltered acceleration values of the upper rib in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel that contains the unfiltered acceleration values of the spine, in gn (gravity acceleration).</td></tr>
<tr><td width="150">[FIR100SampleType]</td>
<td>Specifies whether DIAdem oversamples the 1600 Hz time channel back to the original sample rate in FIR100 filtering. The default value for the <span class="Monospace">FIR100SampleType</span> variable is <span class="Monospace">NoOversample</span>.<div id="exp_FIR100SampleType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NoOversample"</pre></donottranslate></td>
<td>No oversample</td></tr>
<tr><td width="150"><donottranslate><pre>"Oversample"</pre></donottranslate></td>
<td>Oversample</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">TTIRes</td><td>Receives the result of the TTI calculation.<div id="exp_TTIRes">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">TTIVersion</td><td>Receives the version number of the TTI calculation routine.<div id="exp_TTIVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnTTICalc.htm`*
