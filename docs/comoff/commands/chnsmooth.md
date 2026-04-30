---
title: "ChnSmooth"
description: "Uses the floating arithmetic mean or the floating median to smooth a data channel."
---

# ChnSmooth

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSmooth

Uses the floating arithmetic mean or the floating median to smooth a data channel.

## Signature

```python
return_value = dd.ChnSmooth( Y , ResultChannel , SmoothWidth, SmoothType, [SmoothMode])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">SmoothWidth</td>
<td>Specifies the number of neighboring values to the left and right of the channel value that DIAdem uses to calculate the mean.<div id="exp_SmoothWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>1 &lt;= SmoothWidth &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SmoothType</td>
<td>Specifies which neighbor values of the value to be smoothed DIAdem uses for the smoothing process.<div id="exp_SmoothType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"maxNumber"</pre></donottranslate></td>
<td>Maximum number</td></tr>
<tr><td width="150"><donottranslate><pre>"symmetric"</pre></donottranslate></td>
<td>Symmetric distribution</td></tr>
<tr><td width="150"><donottranslate><pre>"leftOnly"</pre></donottranslate></td>
<td>Only previous channel values</td></tr>
</table>
</td></tr>
</table>
<p class="Body">If the distance to the beginning or to the end of the channel is smaller than the one-sided smoothing width N, DIAdem uses the maximum possible number of neighbor values or only smooths symmetrically so that the same number of points are used on either side of the channel value. You can also specify that DIAdem only uses the channel values before the channel value to be smoothed.</p>
</div></td></tr>
<tr><td width="150">[SmoothMode]</td>
<td>Specifies how DIAdem smooths the data channel. The default value is <span class="Monospace">byMeanValue</span>, which means that DIAdem uses the arithmetic mean.<div id="exp_SmoothMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"byMeanValue"</pre></donottranslate></td>
<td>Arithmetic mean</td></tr>
<tr><td width="150"><donottranslate><pre>"byMedian"</pre></donottranslate></td>
<td>Median</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnSmooth("Group/Channel1","Group/Channel3",10,"maxNumber")
```

---

*Source: `ComOff/ChnSmooth.htm`*
