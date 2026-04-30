---
title: "MatVRow"
description: "Multiplies a matrix rowwise by a vector."
---

# MatVRow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatVRow

Multiplies a matrix rowwise by a vector.

## Signature

```python
dd.MatVRow(ChnList, X )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the channels that belong to the matrix are not the same length, DIAdem uses the shortest channel length.</td></tr></table>
</div>

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
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the vector.</td></tr>
</table>
</div>

---

*Source: `ComOff/MatVRow.htm`*
