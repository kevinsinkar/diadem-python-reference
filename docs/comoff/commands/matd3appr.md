---
title: "MatD3Appr"
description: "Uses a setup function to approximate a surface for three-dimensional matrix data."
---

# MatD3Appr

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatD3Appr

Uses a setup function to approximate a surface for three-dimensional matrix data.

## Signature

```python
return_value = dd.MatD3Appr( X , Y , ChnList, ResultChannel , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The <a href="../d3appransatzoff/">D3ApprAnsatzOff</a> command clears the checkboxes of the setup function.</td>
</tr>
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You can assign a maximum of 10 setup functions to the <span class="Monospace">D3ApprAnsatzFct</span> variable.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  <strong></strong>For information about organizing three dimensional data, refer to <a href="#" data-unresolved="1">Organizing 3D Data</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">1</span> index specifies the x-evaluation points and the <span class="Monospace">2</span> index specifies the y-evaluation points.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the variables <a href="../../../varoff/variables/d3gridpolyg/">D3GridPolyg</a>, <a href="../../../varoff/variables/d3gridpolygchn/">D3GridPolygChn</a>, and <a href="../../../varoff/variables/d3gridpolygconv/">D3GridPolygConv</a> to specify the section.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">ChnList</span> variable contains the z-matrix.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <a href="../d3appransatzoff/">D3ApprAnsatzOff</a> command clears the checkboxes of the setup function.</td></tr></table>
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
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the surface.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the surface.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels with the x- and y-values of the matrix. DIAdem generates the result depending on the variable <span class="Monospace">D3StrucOut</span> in triple or matrix structure. If the result is a matrix, DIAdem saves the z-values in the result channels <span class="Monospace">3DApproximatedZ1</span> to 3DApproximated<span class="Monospace">Zn</span>. If the result is a triplet, DIAdem saves the result channel in <span class="Monospace">3DApproximatedZ</span>. DIAdem always saves the z-channels in the default group. The distance between the approximated surface and the specified values is minimal. DIAdem uses the Gauss method of least squares for approximation. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
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
dd.D3ApprAnsatzOff()
dd.D3ApprAnsatzFct[1] = "Yes" # Activates function term constant
dd.D3ApprAnsatzFct[2] = "Yes" # Activates function term x
dd.D3ApprAnsatzFct[3] = "Yes" # Activates function term x^2
dd.D3ApprAnsatzFct[12] = "Yes" # Activates function term y
dd.D3ApprAnsatzFct[13] = "Yes" # Activates function term y^2
dd.D3ApprAnsatzFct[14] = "Yes" # Activates function term y^3
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.MatD3Appr(oMyXChannel, oMyYChannel, oMyChannelList, "Results/3DApproximatedX", "Results/3DApproximatedY")
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
dd.D3ApprAnsatzOff()
dd.D3ApprAnsatzFct[1] = "Yes" # Activates function term constant
dd.D3ApprAnsatzFct[2] = "Yes" # Activates function term x
dd.D3ApprAnsatzFct[3] = "Yes" # Activates function term x^2
dd.D3ApprAnsatzFct[12] = "Yes" # Activates function term y
dd.D3ApprAnsatzFct[13] = "Yes" # Activates function term y^2
dd.D3ApprAnsatzFct[14] = "Yes" # Activates function term y^3
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.MatD3Appr("[2]/[1]", "[2]/[2]", oMyChannelList, "Results/3DApproximatedX", "Results/3DApproximatedY")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/MatD3Appr.htm`*
