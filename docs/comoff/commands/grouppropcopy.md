---
title: "GroupPropCopy"
description: "Copies group properties to another group. You also can use the object-oriented interface to access internal data. Use the AddProperties Properties method to imp"
---

# GroupPropCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GroupPropCopy

Copies group properties to another group. You also can use the object-oriented interface to access internal data. Use the AddProperties Properties method to implement the functionality of the GroupPropCopy command with the script interface for internal data.

## Signature

```python
dd.GroupPropCopy(SourceGroupIndex, TargetGroupIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If a command generates a channel group, specify the value 0 to create a channel group after the last channel group.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The <span class="Monospace">GroupPropCopy</span> command does not copy the channel name, calculated properties, and management properties.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SourceGroupIndex</td>
<td>Specifies the index of a channel group in the Data Portal.<div id="exp_SourceGroupIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr>
<td>1 &lt;= SourceGroupIndex &lt;= <a href="../../../varoff/variables/groupcount/">GroupCount</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">TargetGroupIndex</td>
<td>Specifies the index of a target channel group in the Data Portal.<div id="exp_TargetGroupIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= TargetGroupIndex &lt;= <a href="../../../varoff/variables/groupcount/">GroupCount</a></td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If a command generates a channel group, specify the value 0 to create a channel group after the last channel group.</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/GroupPropCopy.htm`*
