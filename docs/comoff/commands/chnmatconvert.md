---
title: "ChnMatConvert"
description: "Converts a data triplet from an x, y and z-channel into a matrix structure."
---

# ChnMatConvert

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnMatConvert

Converts a data triplet from an x, y and z-channel into a matrix structure.

## Signature

```python
return_value = dd.ChnMatConvert( X , Y , Z , ResultChannel , ResultChannel , D3ConvertTolMode, D3ConvertTol, D3ConvertTolAbsX, D3ConvertTolAbsY, [D3ConvertRedMode])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> If the tolerance you select is too high, DIAdem combines values with a greater difference to one value. If the tolerance is too small, DIAdem assigns identical numbers to different representatives.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> If the tolerance you select is too high, DIAdem combines values with a greater difference to one value. If the tolerance is too small, DIAdem assigns identical numbers to different representatives.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> If the tolerance you select is too high, DIAdem combines values with a greater difference to one value. If the tolerance is too small, DIAdem assigns identical numbers to different representatives.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>Z</em></td>
<td>Specifies the data channel containing the z-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the x-values of the matrix.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the y-values of the matrix.</td></tr>
<tr><td width="150">D3ConvertTolMode</td>
<td>Specifies whether DIAdem checks the similarity of two value pairs using relative or absolute exactness.<div id="exp_D3ConvertTolMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"relative"</pre></donottranslate></td>
<td>Relative</td></tr>
<tr><td width="150"><donottranslate><pre>"absolute"</pre></donottranslate></td>
<td>Absolute</td></tr>
</table>
</td></tr>
</table>
<p class="Body">DIAdem checks for equality while allowing for a <a href="../../../varoff/variables/d3converttol/">Tolerance</a>.</p>
</div></td></tr>
<tr><td width="150">D3ConvertTol</td>
<td>Specifies the tolerance as a percentage within which DIAdem combines value pairs into single values.<div id="exp_D3ConvertTol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= D3ConvertTol &lt;= 10</td></tr>
</table>
<p class="Body">The tolerance in percentage specifies how accurately DIAdem checks the values for equality. The check compensates inaccuracies in measurements when DIAdem converts from triplet to matrix.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> If the tolerance you select is too high, DIAdem combines values with a greater difference to one value. If the tolerance is too small, DIAdem assigns identical numbers to different representatives.</td></tr></table>
</div></td></tr>
<tr><td width="150">D3ConvertTolAbsX</td>
<td>Specifies the absolute tolerance within which DIAdem combines x-values into a single value.<div id="exp_D3ConvertTolAbsX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1E-9 &lt;= D3ConvertTolAbsX &lt;= 1E300</td></tr>
</table>
<p class="Body">The absolute tolerance specifies how accurately DIAdem checks the x-values for equality. The check compensates inaccuracies in measurements when DIAdem converts from triplet to matrix.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> If the tolerance you select is too high, DIAdem combines values with a greater difference to one value. If the tolerance is too small, DIAdem assigns identical numbers to different representatives.</td></tr></table>
</div></td></tr>
<tr><td width="150">D3ConvertTolAbsY</td>
<td>Specifies the absolute tolerance within which DIAdem combines y-values into a single value.<div id="exp_D3ConvertTolAbsY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1E-9 &lt;= D3ConvertTolAbsY &lt;= 1E300</td></tr>
</table>
<p class="Body">The absolute tolerance specifies how accurately DIAdem checks the y-values for equality. The check compensates inaccuracies in measurements when DIAdem converts from triplet to matrix.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> If the tolerance you select is too high, DIAdem combines values with a greater difference to one value. If the tolerance is too small, DIAdem assigns identical numbers to different representatives.</td></tr></table>
</div></td></tr>
<tr><td width="150">[D3ConvertRedMode]</td>
<td>Specifies how DIAdem combines three-dimensional data when DIAdem converts a triplet to a matrix. By default the <span class="Monospace">D3ConvertRedMode</span> variable contains the value <span class="Monospace">mean</span>.<div id="exp_D3ConvertRedMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"minimum"</pre></donottranslate></td>
<td>Minimum</td></tr>
<tr><td width="150"><donottranslate><pre>"maximum"</pre></donottranslate></td>
<td>Maximum</td></tr>
<tr><td width="150"><donottranslate><pre>"mean"</pre></donottranslate></td>
<td>Mean value</td></tr>
<tr><td width="150"><donottranslate><pre>"sum"</pre></donottranslate></td>
<td>Sum</td></tr>
<tr><td width="150"><donottranslate><pre>"first value"</pre></donottranslate></td>
<td>First value</td></tr>
<tr><td width="150"><donottranslate><pre>"last value"</pre></donottranslate></td>
<td>Last value</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels with the x- and y-values of the matrix. DIAdem saves the result matrix in the default group. If DIAdem cannot assign a value from the z-channel to an element of the z-matrix during conversion, this matrix element receives <a href="#" data-unresolved="1">NoValue</a>. The return value is an <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyZChannel = dd.Data.Root.ChannelGroups(2).Channels(3)
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnMatConvert(oMyXChannel, oMyYChannel, oMyZChannel, "Results/ConvertedMatrixX", "Results/ConvertedMatrixY", "relative", 0.01, 1, 1, "mean")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.ChnMatConvert("[2]/[1]", "[2]/[2]", "[2]/[3]", "Results/ConvertedMatrixX", "Results/ConvertedMatrixY" ,"relative", 0.01, 1, 1, "mean")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnMatConvert.htm`*
