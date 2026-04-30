---
title: "MatMul"
description: "Multiplies two matrices."
---

# MatMul

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatMul

Multiplies two matrices.

## Signature

```python
dd.MatMul(ChnList1, ChnList2, MatMulType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  For algebraic multiplication the number of columns of the first matrix must be the same as the number of rows of the second matrix.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  For componentwise multiplication both matrices must be the same size.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>A <span class="Monospace">NoValue</span> in a matrix component results in a <span class="Monospace">NoValue</span> in the result matrix.</td></tr></table>
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
<tr><td width="150">MatMulType</td>
<td>Specifies whether DIAdem multiplies the matrices componentwise or algebraically.<div id="exp_MatMulType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"algebraic"</pre></donottranslate></td>
<td>Algebraic</td></tr>
<tr><td width="150"><donottranslate><pre>"by components"</pre></donottranslate></td>
<td>Componentwise</td></tr>
</table>
</td></tr>
</table><strong><p class="Body">Algebraic</p></strong><p class="Body"><img border="0" height="73" src="image/m_3D_10.gif" width="582"/></p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  For algebraic multiplication the number of columns of the first matrix must be the same as the number of rows of the second matrix.</td></tr></table><strong><p class="Body">Componentwise</p></strong><p class="Body"><img border="0" height="73" src="image/m_3D_08.gif" width="393"/></p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  For componentwise multiplication both matrices must be the same size.</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/MatMul.htm`*
