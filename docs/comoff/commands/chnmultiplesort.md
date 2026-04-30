---
title: "ChnMultipleSort"
description: "Sorts values in data channels in ascending order. DIAdem sorts texts according to the ASCII table."
---

# ChnMultipleSort

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnMultipleSort

Sorts values in data channels in ascending order. DIAdem sorts texts according to the ASCII table.

## Signature

```python
dd.ChnMultipleSort(CALCXChn, CALCYChn, SortSwitch, [ChnMSortIP])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not overwrite the result channels, DIAdem saves the result channels in the default group.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CALCXChn</td>
<td>Specifies the data channel with the x-values of the signal.<div id="exp_CALCXChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CALCYChn</td>
<td>Specifies the data channels containing the y-values of the signal.<div id="exp_CALCYChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">SortSwitch</td>
<td>Specifies whether DIAdem only sorts the first data channel.<div id="exp_SortSwitch">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnMSortIP]</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the sorting result values. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not overwrite the input channels.<div id="exp_ChnMSortIP">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.ChnMultipleSort("Group1/Control", oMyChannelList, False, False)
```

---

*Source: `ComOff/ChnMultipleSort.htm`*
