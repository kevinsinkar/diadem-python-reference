---
title: "MatD3Interp"
description: "Calculates a three-dimensional interpolation for an x-channel, a y-channel, and a z-matrix."
---

# MatD3Interp

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatD3Interp

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

Calculates a three-dimensional interpolation for an x-channel, a y-channel, and a z-matrix.

## Signature

```python
return_value = dd.MatD3Interp( X , Y , ChnList, ResultChannel , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  <strong></strong>For information about organizing three-dimensional data, refer to <a href="#" data-unresolved="1">Organizing 3D Data</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  <strong></strong>For information about organizing three dimensional data, refer to <a href="#" data-unresolved="1">Organizing 3D Data</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the variables <a href="../../../varoff/variables/d3gridpolyg/">D3GridPolyg</a>, <a href="../../../varoff/variables/d3gridpolygchn/">D3GridPolygChn</a>, and <a href="../../../varoff/variables/d3gridpolygconv/">D3GridPolygConv</a> to specify the section.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note</strong>  The dialog box offers you the SISPL and SCADI procedures, while you can also use the other interpolation procedures in the script.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note</strong>  DIAdem only uses the <span class="Monospace">D3InterpPara(2)</span> variable internally.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the interpolation.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the interpolation.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels with the x- and y-values of the interpolation. DIAdem generates the result depending on the variable <span class="Monospace">D3StrucOut</span> in triple or matrix structure. If it is a matrix, DIAdem saves the z-values in the result channels <span class="Monospace">3DInterpolatedZ1</span> to <span class="Monospace">3DInterpolatedZn</span>. If it is a triplet, DIAdem saves the result channel in <span class="Monospace">3DInterpolatedZ</span>. DIAdem always saves the z-channels in the default group. In each internal grid point DIAdem calculates a bicubic polynomial on the basis of the surrounding grid points and calculates a biquadratic polynomial in each boundary point. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
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
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.MatD3Interp(oMyXChannel, oMyYChannel, oMyChannelList, "Results/3DInterpolatedX", "Results/3DInterpolatedY")
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
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.MatD3Interp("[2]/[1]", "[2]/[2]", oMyChannelList, "Results/3DInterpolatedX", "Results/3DInterpolatedY")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/MatD3Interp.htm`*
