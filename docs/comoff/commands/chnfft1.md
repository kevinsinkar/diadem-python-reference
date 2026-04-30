---
title: "ChnFFT1"
description: "Executes a fast Fourier transform (FFT) of a signal."
---

# ChnFFT1

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFFT1

Executes a fast Fourier transform (FFT) of a signal.

## Signature

```python
return_value = dd.ChnFFT1( XW , ChnList)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can generate an index channel if you calculate the FFT over several channels or time intervals and if you do not run an averaging.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you assign the value <span class="Monospace">all</span> to the variables <span class="Monospace">FFTIntervUser</span> or <span class="Monospace">LengthStartOverl</span>, DIAdem checks the interval length you selected. If the interval is longer than the channel, DIAdem corrects the interval length to the greatest power of two below the channel length.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You need at least two sampling points per oscillation to obtain worthwhile results. Select the sampling rate of the time signal and the number of sampling points according to the respective frequency domain. Because real-time functions have an amplitude spectrum that is axis-symmetrical and periodic with the sampling frequency, N real-time values can be adequately represented in Fourier analysis by N/2 complex values in the frequency domain.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values of the signal. The data channel must not contain NoValues and the values of the data channel must be strictly monotonic increasing and equidistant.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. DIAdem generates at least two result channels in the default group. The first result channel contains the frequency. The other result channels contain the values for the selected analysis functions. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnFFT1.htm`*
