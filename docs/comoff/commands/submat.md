---
title: "SubMat"
description: "Extracts a submatrix from a matrix."
---

# SubMat

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SubMat

Extracts a submatrix from a matrix.

## Signature

```python
return_value = dd.SubMat( X , Y , ChnList, ResultChannel , ResultChannel , D3SubMatRow, D3SubMatColumn, D3SubMatTranspos)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Specify which columns of a submatrix you want to copy with the <a href="../../../varoff/variables/d3submatrow/">D3SubMatColumn</a> variable.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Specify which rows of a submatrix you want to copy with the <a href="../../../varoff/variables/d3submatrow/">D3SubMatRow</a> variable.</td></tr></table>
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
<td>Specifies the result channel for the x-values of the submatrix.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the y-values of the submatrix.</td></tr>
<tr><td width="150">D3SubMatRow</td>
<td>Specifies which rows to copy from a submatrix.<div id="exp_D3SubMatRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Specify which columns of a submatrix you want to copy with the <a href="../../../varoff/variables/d3submatrow/">D3SubMatColumn</a> variable.</td></tr></table>
<h2>Examples</h2>
<p class="Body">The following settings are valid for the <span class="Monospace">D3SubMatRow</span> variable:</p>
<table class="border1ess">
<tr>
<td width="150"><span class="Monospace">3,6-9,14</span></td>
<td>Copies the rows 3, 6-9, and 14</td>
</tr>
<tr>
<td width="150"><span class="Monospace">3-</span></td>
<td>Copies all rows from the third to the last row.</td>
</tr>
<tr>
<td width="150"><span class="Monospace">-6</span></td>
<td>Copies all rows from the first to the sixth row.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">D3SubMatColumn</td>
<td>Specifies which columns to copy from a submatrix.<div id="exp_D3SubMatColumn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Specify which rows of a submatrix you want to copy with the <a href="../../../varoff/variables/d3submatrow/">D3SubMatRow</a> variable.</td></tr></table>
<h2>Examples</h2>
<p class="Body">The following settings are valid for the <span class="Monospace">D3SubMatColumn</span> variable:</p>
<table class="border1ess">
<tr>
<td width="150"><span class="Monospace">3,6-9,14</span></td>
<td>Copies the columns 3, 6-9, and 14</td>
</tr>
<tr>
<td width="150"><span class="Monospace">3-</span></td>
<td>Copies all columns from the third to the last column.</td>
</tr>
<tr>
<td width="150"><span class="Monospace">-6</span></td>
<td>Copies all columns from the first to the sixth column.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">D3SubMatTranspos</td>
<td>Specifies whether DIAdem transposes and saves rows and columns in a submatrix.<div id="exp_D3SubMatTranspos">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If you extract a submatrix with few rows but many columns, store the submatrix in the transposed mode.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels with the x- and y-values of the submatrix. DIAdem always saves the z-channels in the default group. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
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
oMyResultChn = dd.SubMat(oMyXChannel, oMyYChannel, oMyChannelList, "Results/PartialMatrixX", "Results/PartialMatrixY", "1-4", "3-", False)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyChannelList = dd.Data.GetChannels("[2]/Z*")
if not(dd.Data.Root.ChannelGroups.Exists("Results")) :
    dd.Data.Root.ChannelGroups.Add("Results")
dd.Data.Root.ChannelGroups.Item("Results").Activate()
oMyResultChn = dd.SubMat("[2]/[1]", "[2]/[2]", oMyChannelList, "Results/PartialMatrixX", "Results/PartialMatrixY", "1-4", "3-", False)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/SubMat.htm`*
