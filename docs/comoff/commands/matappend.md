---
title: "MatAppend"
description: "Appends a matrix to a matrix."
---

# MatAppend

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatAppend

Appends a matrix to a matrix.

## Signature

```python
dd.MatAppend( X1 , Y1 , ChnList1, X2 , ChnList2)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The x-channel and the z-channels of the first matrix must be the same length.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the channels in the second matrix are not the same length, DIAdem only appends the values of the smallest common channel length to the original matrix.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem overwrites the original matrix with the result matrix.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel containing the x-values of the first matrix.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the y-values of the first matrix.</td></tr>
<tr><td width="150">ChnList1</td>
<td>Specifies one or more channels.<div id="exp_ChnList1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>X2</em></td>
<td>Specifies the data channel containing the x-values of the second matrix.</td></tr>
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

*Source: `ComOff/MatAppend.htm`*
