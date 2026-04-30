---
title: "MatVAlgebr"
description: "Multiplies a matrix algebraically by a vector."
---

# MatVAlgebr

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatVAlgebr

Multiplies a matrix algebraically by a vector.

## Signature

```python
return_value = dd.MatVAlgebr(ChnList, X , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the channels that belong to the matrix are not the same length, DIAdem uses the shortest channel length.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the vector.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the result vector.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel with the result vector. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyResultChn = dd.MatVAlgebr(oMyChannelList, oMyYChannel, "Results/MatrixVectorProduct")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyResultChn = dd.MatVAlgebr(oMyChannelList, "[2]/[2]", "Results/MatrixVectorProduct")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/MatVAlgebr.htm`*
