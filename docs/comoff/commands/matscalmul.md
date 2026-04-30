---
title: "MatScalMul"
description: "Multiplies a matrix componentwise by a scalar value."
---

# MatScalMul

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatScalMul

Multiplies a matrix componentwise by a scalar value.

## Signature

```python
dd.MatScalMul(ChnList, MatScalVal, MatScalIP)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The number of rows in the matrix must correspond to the length of the first channel and the number columns in the matrix must correspond to the length of the second channel. If not, DIAdem uses the maximum possible dimension for the calculation.</td></tr></table>
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
<tr><td width="150">MatScalVal</td>
<td>Specifies the scalar value that DIAdem uses to add or to multiply the matrix componentwise.<div id="exp_MatScalVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MatScalIP</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result values of the matrix operation.<div id="exp_MatScalIP">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/MatScalMul.htm`*
