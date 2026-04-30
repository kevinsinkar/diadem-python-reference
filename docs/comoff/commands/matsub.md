---
title: "MatSub"
description: "Subtracts two matrices componentwise."
---

# MatSub

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatSub

Subtracts two matrices componentwise.

## Signature

```python
dd.MatSub(ChnList1, ChnList2)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>A <span class="Monospace">NoValue</span> in a matrix component results in a <span class="Monospace">NoValue</span> in the result matrix.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the two matrices do not have the same number of columns and rows, DIAdem uses the lowest common number of columns and rows.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ChnList2</td>
<td>Specifies one or more channels.<div id="exp_ChnList2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/MatSub.htm`*
