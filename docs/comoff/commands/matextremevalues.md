---
title: "MatExtremeValues"
description: "Determines the minimum value and the maximum value of a matrix."
---

# MatExtremeValues

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatExtremeValues

Determines the minimum value and the maximum value of a matrix.

## Signature

```python
dd.MatExtremeValues(ChnList, MatExtCheckPos)
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
<tr><td width="150">MatExtCheckPos</td>
<td>Specifies whether DIAdem determines the columns and rows that contain the extreme values.<div id="exp_MatExtCheckPos">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">MatMin</td><td>Receives the minimum value of a matrix.<div id="exp_MatMin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MatMax</td><td>Receives the maximum value of a matrix.<div id="exp_MatMax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MatMinCol</td><td>Receives the column number of the minimum value of a matrix.<div id="exp_MatMinCol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MatMinRow</td><td>Receives the row number of the minimum value of a matrix.<div id="exp_MatMinRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MatMaxCol</td><td>Receives the column number of the maximum value of a matrix.<div id="exp_MatMaxCol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MatMaxRow</td><td>Receives the row number of the maximum value of a matrix.<div id="exp_MatMaxRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/MatExtremeValues.htm`*
