---
title: "ChnConcatenateGroupsWithPadding"
description: "Adds all channels from selected groups to the channels of the base group. DIAdem concatenates channels with the same name. To bring all channels to the same len"
---

# ChnConcatenateGroupsWithPadding

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConcatenateGroupsWithPadding

Adds all channels from selected groups to the channels of the base group. DIAdem concatenates channels with the same name. To bring all channels to the same length, DIAdem adds NoValues to the channels that are not contained in all groups.

## Signature

```python
return_value = dd.ChnConcatenateGroupsWithPadding( ChnConcatenateBaseGroup , ChnConcatenateSourceGroups , ChnConcatenateMarkBoundaries)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnConcatenateBaseGroup</td>
<td>Specifies the channel group to which DIAdem adds channels from other groups and appends channels with the same name.<div id="exp_ChnConcatenateBaseGroup">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnConcatenateSourceGroups</td>
<td>Specifies the channel groups containing the channels DIAdem concatenates or adds to the channels of the base group. The order of the channel group specifies the order in which DIAdem concatenates or adds the channels to the base channels. You can only concatenate data channels of the same type.<div id="exp_ChnConcatenateSourceGroups">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<p class="body">For the <span class="Monospace">ChnConcatenateGroups</span> command, channels with the same names as in the base group or with the same number of channels must be in the channel groups you want to concatenate.</p>
<p class="body">For the <span class="Monospace">ChnConcatenateGroupsAdjustment</span> command, the channel groups can also contain channels that do not exist in the base group. DIAdem supplements the missing group sections in the channels with <span class="Monospace">NoValues</span>.</p>
</div></td></tr>
<tr><td width="150">ChnConcatenateMarkBoundaries</td>
<td>Specifies that DIAdem inserts a separator after each channel to make the original channels visible. DIAdem inserts <span class="Monospace">NoValue</span> for numeric channels and the following character:<span class="Monospace"> .---.-.</span> for text channels.<div id="exp_ChnConcatenateMarkBoundaries">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels and the new channel group. The number of channels corresponds to the sum of all channels of all channel groups. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyBaseGroup = dd.Data.Root.ChannelGroups(1)
oMyConcatGroups = dd.Data.CreateElementList()
oMyConcatGroups.Add(dd.Data.Root.ChannelGroups(2))
oMyConcatGroups.Add(dd.Data.Root.ChannelGroups(3))
oMyResultChn = dd.ChnConcatenateGroupsWithPadding(oMyBaseGroup, oMyConcatGroups, True, False)
print("Results in Group: " , oMyResultChn(1).ChannelGroup.Name)
```

```python
oMyResultChn = dd.ChnConcatenateGroupsWithPadding("Group1", "'Group2','Group3'", True, False)
print("Results in Group: " , oMyResultChn(1).ChannelGroup.Name)
```

---

*Source: `ComOff/ChnConcatenateGroupsWithPadding.htm`*
