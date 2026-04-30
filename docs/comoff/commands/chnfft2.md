---
title: "ChnFFT2"
description: "Executes a fast Fourier transform (FFT) of two signals with a common time channel."
---

# ChnFFT2

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFFT2

Executes a fast Fourier transform (FFT) of two signals with a common time channel.

## Signature

```python
dd.ChnFFT2( XW , ChnList1, ChnList2)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can generate an index channel if you calculate the FFT over several channels or time intervals and if you do not run an averaging.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you assign the value <span class="Monospace">all</span> to the variables <span class="Monospace">FFTIntervUser</span> or <span class="Monospace">LengthStartOverl</span>, DIAdem checks the interval length you selected. If the interval is longer than the channel, DIAdem corrects the interval length to the greatest power of two below the channel length.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You need at least two sampling points per oscillation to obtain worthwhile results. Select the sampling rate of the time signal and the number of sampling points in such a way that the specified frequency domain is described properly. Because real-time functions have an amplitude spectrum that is axis-symmetrical and periodic with the sampling frequency, N real-time values can be adequately represented in Fourier analysis by N/2 complex values in the frequency domain.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the signals. The values of the data channel must be equidistant and monotonic increasing.</td></tr>
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ChnList2</td>
<td>Specifies one or more channels.<div id="exp_ChnList2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnFFT2.htm`*
