---
title: "ToVirtGridCtrl.Visible"
description: "Specifies in user dialog boxes whether a column of the extended table is visible."
---

# ToVirtGridCtrl.Visible

!!! abstract "Property &middot; `Sudref.chm`"
    Property: Visible for XTable

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

Specifies in user dialog boxes whether a column of the extended table is visible.

## Signature

```python
obj.Visible
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <a href="../../events/eventvalget-eventvalget/">EventValGet</a> event is only triggered for visible cells.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
XTable1.Columns(3).Visible = 0  # 0=No, 1=Yes
```

---

*Source: `Sudref/properties/SUD_property_Visible_ToVirtGridCtrl.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
