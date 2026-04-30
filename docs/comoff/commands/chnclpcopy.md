---
title: "ChnClpCopy"
description: "Copies channels to the clipboard."
---

# ChnClpCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnClpCopy

Copies channels to the clipboard.

## Signature

```python
dd.ChnClpCopy(ClpSource, [ ChnXYRelation ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Avoid using the Windows clipboard in scripts, especially in loops. Timely access to the clipboard is unpredictable and may lead to unexpected behavior. Use the <a href="../chncopy/">ChnCopy</a> command to copy channels directly.<br attr="ext"/>When you copy and paste a calculation channel, DIAdem first deletes all calculated data, the unit and, if available, the xy relationship. When you update values in the Data Portal, DIAdem attempts to recalculate the values with the channels in the channel group and restore the xy relationship. This is only possible if the specified channels are available in the channel group. Use the <a href="../../../inavidata/methods/idiademcalculationchannel-runcalculation/">RunCalculation for CalculationChannel</a> method to calculate the values of of a calculation channel.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ClpSource</td>
<td>Specifies one or more channels.<div id="exp_ClpSource">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">[ChnXYRelation]</td>
<td>Specifies that x-channel references are used when copying and moving xy-channels and are preserved during reduced loading of xy-channels.<div id="exp_ChnXYRelation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("[1]/Channel*")
oMyChannelList.Add(dd.Data.Root.ChannelGroups(2))
dd.ChnClpCopy(oMyChannelList)
```

---

*Source: `ComOff/ChnClpCopy.htm`*
