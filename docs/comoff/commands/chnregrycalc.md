---
title: "ChnRegrYCalc"
description: "Uses a regression function to approximate a signal."
---

# ChnRegrYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRegrYCalc

Uses a regression function to approximate a signal.

## Signature

```python
return_value = dd.ChnRegrYCalc( XW , Y , SamplingPointChn, ResultChannel , RegrType)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal. The y-channel you want to evaluate must not contain negative values when DIAdem uses a logarithmic setup function.</td></tr>
<tr><td width="150">SamplingPointChn</td>
<td>Specifies the data channel containing the interpolation points.<div id="exp_SamplingPointChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the regression function.</td></tr>
<tr><td width="150">RegrType</td>
<td>Specifies the setup function for a regression.<div id="exp_RegrType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"linear"</pre></donottranslate></td>
<td>Linear</td></tr>
<tr><td width="150"><donottranslate><pre>"power"</pre></donottranslate></td>
<td>Power</td></tr>
<tr><td width="150"><donottranslate><pre>"exponential"</pre></donottranslate></td>
<td>Exponential</td></tr>
<tr><td width="150"><donottranslate><pre>"logarith.10"</pre></donottranslate></td>
<td>Decadic logarithm</td></tr>
<tr><td width="150"><donottranslate><pre>"logarith.n"</pre></donottranslate></td>
<td>Natural logarithm</td></tr>
<tr><td width="150"><donottranslate><pre>"power no weight adjustment"</pre></donottranslate></td>
<td>Power (without weight adjustment)</td></tr>
<tr><td width="150"><donottranslate><pre>"exponential no weight adjustment"</pre></donottranslate></td>
<td>Exponential (without weight adjustment)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel containing the y-values of the regression function. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyY1Channel = dd.Data.Root.ChannelGroups(1).Channels(3)
oMyResultChn = dd.ChnRegrYCalc(oMyXChannel, oMyYChannel, oMyY1Channel, "Results/RegressionY", "linear")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyResultChn = dd.ChnRegrYCalc("[1]/[1]", "[1]/[2]", "[1]/[3]", "Results/RegressionY", "linear")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnRegrYCalc.htm`*
