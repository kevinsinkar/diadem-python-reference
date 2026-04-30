---
title: "MatSort"
description: "Sorts the values of the x and of the y-channel in a matrix monotonic increasing. DIAdem transposes the z-matrix values according to the new order."
---

# MatSort

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatSort

Sorts the values of the x and of the y-channel in a matrix monotonic increasing. DIAdem transposes the z-matrix values according to the new order.

## Signature

```python
return_value = dd.MatSort( X , Y , ChnList, ResultChannel , ResultChannel , [MatSortIP])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The number of rows of the z-matrix must correspond to the length of the x-channel and the number of columns of the z-matrix must correspond to the length of the y-channel. If not, DIAdem uses the maximum possible dimension for the calculation.</td></tr></table>
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
<td>Specifies the result channel for the x-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the y-values.</td></tr>
<tr><td width="150">[MatSortIP]</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the sorting result values. The default value is <span class="Monospace">False</span> which specifies that DIAdem does not overwrite the input channels.<div id="exp_MatSortIP">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels with the x- and y-values of the sorted matrix. DIAdem always saves the z-channels in the default group. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.MatSort(oMyXChannel, oMyYChannel, oMyChannelList, "Results/SortedMatrixX", "Results/SortedMatrixY", False)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.MatSort("[2]/[1]", "[2]/[2]", oMyChannelList, "Results/SortedMatrixX", "Results/SortedMatrixY", False)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/MatSort.htm`*
