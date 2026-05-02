---
title: "ChnD3Interp"
description: "Calculates a three-dimensional interpolation for a data triplet with x, y and z-channels."
---

# ChnD3Interp

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnD3Interp

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('D3StrucOut', ...)   # instead of dd.D3StrucOut = ...
    bridge.IntegerVarSet('D3GridCalcAll', ...)   # instead of dd.D3GridCalcAll = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Calculates a three-dimensional interpolation for a data triplet with x, y and z-channels.

## Signature

```python
return_value = dd.ChnD3Interp( X , Y , Z , ResultChannel , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  <strong></strong>For information about organizing three dimensional data, refer to <a href="#" data-unresolved="1">Organizing 3D Data</a>.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note</strong>  DIAdem only uses the <span class="Monospace">D3InterpPara(2)</span> variable internally.</td>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the variables <a href="../../../varoff/variables/d3gridpolyg/">D3GridPolyg</a>, <a href="../../../varoff/variables/d3gridpolygchn/">D3GridPolygChn</a>, and <a href="../../../varoff/variables/d3gridpolygconv/">D3GridPolygConv</a> to specify the section.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem generates the result as a triplet or a matrix depending on the <span class="Monospace">D3StrucOut</span> variable. If it is a matrix, DIAdem saves the z-values in the result channels <span class="Monospace">D3InterpZ1</span> to <span class="Monospace">D3InterpZn</span>. If it is a triplet, DIAdem saves the result channel in <span class="Monospace">D3InterpZ</span>. DIAdem always saves the z-channels in the default group.</td></tr></table>
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
<td>Specifies the result channel that contains the x-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that contains the y-values.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels. The first result channel contains the x-values and the second result channel contains the y-values of the interpolation function. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.D3StrucOut = "Matrix"
dd.D3GridGen[1] = "calculated"
dd.D3GridCalc[1] = "automatic"
dd.D3GridNo[1] = 20
dd.D3GridGen[2] = "calculated"
dd.D3GridCalc[2] = "automatic"
dd.D3GridNo[2] = 25
dd.D3GridCalcAll = 0
dd.D3GridPolyg = "convex hull"
dd.D3NodeMeth = "n neigh. pts"
dd.D3NodeNo = 5
dd.D3InterpMethChn = "SCADI"
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyZChannel = dd.Data.Root.ChannelGroups(2).Channels(3)
oMyResultChn = dd.ChnD3Interp(oMyXChannel, oMyYChannel, oMyZChannel, "Results/3DApproximatedX", "Results/3DApproximatedY")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
dd.D3StrucOut = "Matrix"
dd.D3GridGen[1] = "calculated"
dd.D3GridCalc[1] = "automatic"
dd.D3GridNo[1] = 20
dd.D3GridGen[2] = "calculated"
dd.D3GridCalc[2] = "automatic"
dd.D3GridNo[2] = 25
dd.D3GridCalcAll = 0
dd.D3GridPolyg = "convex hull"
dd.D3NodeMeth = "n neigh. pts"
dd.D3NodeNo = 5
dd.D3InterpMethChn = "SCADI"
oMyResultChn = dd.ChnD3Interp("[2]/[1]", "[2]/[2]", "[2]/[3]", "Results/3DInterpolatedX", "Results/3DInterpolatedY")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnD3Interp.htm`*
