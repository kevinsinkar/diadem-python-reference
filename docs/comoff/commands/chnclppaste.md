---
title: "ChnClpPaste"
description: "Pastes channels from the clipboard to the default group in the Data Portal."
---

# ChnClpPaste

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnClpPaste

Pastes channels from the clipboard to the default group in the Data Portal.

## Signature

```python
dd.ChnClpPaste(ClpTarget, [ ChnXYRelation ])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Avoid using the Windows clipboard in scripts, especially in loops. Timely access to the clipboard is unpredictable and may lead to unexpected behavior. Use the <a href="../../../inavidata/methods/inavidata-move/">Move for Data</a> method to move the inserted channels to the target position in a channel group. Use the <a href="../chncopy/">ChnCopy</a> command to copy channels directly.<br attr="ext"/>When you copy and paste a calculation channel, DIAdem first deletes all calculated data, the unit and, if available, the xy relationship. When you update values in the Data Portal, DIAdem attempts to recalculate the values with the channels in the channel group and restore the xy relationship. This is only possible if the specified channels are available in the channel group. Use the <a href="../../../inavidata/methods/idiademcalculationchannel-runcalculation/">RunCalculation for CalculationChannel</a> method to calculate the values of of a calculation channel.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ClpTarget</td>
<td>Specifies the channel number which the first inserted channel receives. If the target channel number already exists, DIAdem moves the existing channels.<div id="exp_ClpTarget">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
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

---

*Source: `ComOff/ChnClpPaste.htm`*
