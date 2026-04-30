---
title: "MatSum"
description: "Calculates the sum of the rows and the sum of the columns in a matrix."
---

# MatSum

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatSum

Calculates the sum of the rows and the sum of the columns in a matrix.

## Signature

```python
return_value = dd.MatSum(ChnList, ResultChannel , ResultChannel )
```

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
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the sums of the individual rows.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the sums of the individual columns.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels with the sums of the individual rows and columns. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
oMyResultChn = dd.MatSum(oMyChannelList, "Results/MatrixSumRows", "Results/MatrixSumColumns")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/MatSum.htm`*
