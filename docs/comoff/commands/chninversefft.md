---
title: "ChnInverseFFT"
description: "Executes an inverse fast Fourier transform (FFT). DIAdem transforms a signal from the frequency domain into the time domain."
---

# ChnInverseFFT

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnInverseFFT

Executes an inverse fast Fourier transform (FFT). DIAdem transforms a signal from the frequency domain into the time domain.

## Signature

```python
return_value = dd.ChnInverseFFT( XW , X1 , Y1 , ResultChannel , ResultChannel , [IFFTHilbert])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the frequencies of the complex signal. The x-values must be strictly monotone increasing. If all other channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel containing the real part of the signal.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the imaginary part of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the time.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the amplitude.</td></tr>
<tr><td width="150">[IFFTHilbert]</td>
<td>Specifies the phase shift for inverse fast Fourier transform. The default value of the <span class="Monospace">IFFTHilbert</span> variable is <span class="Monospace">No</span>.<div id="exp_IFFTHilbert">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"No"</pre></donottranslate></td>
<td>None</td></tr>
<tr><td width="150"><donottranslate><pre>"90"</pre></donottranslate></td>
<td>90</td></tr>
<tr><td width="150"><donottranslate><pre>"-90"</pre></donottranslate></td>
<td>-90</td></tr>
<tr><td width="150"><donottranslate><pre>"180"</pre></donottranslate></td>
<td>180</td></tr>
</table>
</td></tr>
</table>The setting <span class="Monospace">90</span> is the Hilbert transform. The setting <span class="Monospace">-90</span> is the inverse Hilbert transform.</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels. The first result channel contains the time values and the second result channel contains the amplitude values. The length of the result channels of the inverse FFT is twice as long as the length of the frequency channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyX1Channel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(3)
oMyResultChn = dd.ChnInverseFFT(oMyXChannel, oMyX1Channel, oMyYChannel, "Results/Time", "Results/Amplitude", "No")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyResultChn = dd.ChnInverseFFT("[1]/[1]", "[1]/[2]", "[1]/[3]",  "Results/Time", "Results/Amplitude", "No")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnInverseFFT.htm`*
