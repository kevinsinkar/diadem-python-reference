---
title: "MatIntegrate"
description: "Calculates the volume under a surface that is specified by a matrix."
---

# MatIntegrate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatIntegrate

Calculates the volume under a surface that is specified by a matrix.

## Signature

```python
return_value = dd.MatIntegrate( X , Y , ChnList, ResultChannel , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If an x-value or a y-value is a NoValue, DIAdem also assigns NoValue to the respective component. DIAdem does not include rectangle sections that contain NoValues in the integral calculation.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values of the matrix.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the matrix.</td></tr>
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
<td>Specifies the result channel of the row-wise summation.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel of the column-wise summation.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels. The first result channel contains the values of the row-wise summation and the second result channel contains the values of the column-wise summation. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyResultChn = dd.MatIntegrate(oMyXChannel, oMyYChannel, oMyChannelList, "Results/MatrixIntegratedRows", "Results/MatrixIntegratedColumns")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyResultChn = dd.MatIntegrate("[2]/[1]","[2]/[2]", oMyChannelList, "Results/MatrixIntegratedRows", "Results/MatrixIntegratedColumns")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/MatIntegrate.htm`*
