---
title: "ChnName"
description: "Valid names: ChnName, CN"
---

# ChnName

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ChnName

Valid names: ChnName, CN

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  For information on channel naming, see the <a href="#" data-unresolved="1">Name Conventions</a> page.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
@@ChnName(CurrxChnNo)@@ [@@ChnDim(CurrxChnNo)@@]
```

```python
@@ChnName(dd.Data.GetChannel("[1]/[1]"))@@ [@@ChnDim(dd.Data.GetChannel("[1]/[1]"))@@]
```

```python
@@ChnName("[1]/[1]")@@ [@@ChnDim("[1]/[1]")@@]
```

---

*Source: `VarOff/ChnName.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
