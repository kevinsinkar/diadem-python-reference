---
title: "ChnDim"
description: "Valid names: ChnDim, CD"
---

# ChnDim

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ChnDim

Valid names: ChnDim, CD

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  In REPORT, the <a href="../reportunitdisplaymode/">display mode for the unit for axis labels</a> determines how the unit is displayed in the label text of the axis if it is used in a <a href="#" data-unresolved="1">DIAdem expression</a> within square brackets.</td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
@@ChnName(CurrXChnNo)@@ [@@ChnDim(CurrXChnNo)@@]
```

```python
@@dd.Data.GetChannel("[1]/[1]").Name@@ [@@dd.Data.GetChannel("[1]/[1]").UnitSymbol@@]
```

```python
@@ChnName("[1]/[1]")@@ [@@ChnDim("[1]/[1]")@@]
```

---

*Source: `VarOff/ChnDim.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
