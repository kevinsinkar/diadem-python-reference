---
title: "ToVirtGridCtrl.Right"
description: "Specifies the distance between the right edge of a control and the user dialog box origin. The dialog box origin is in the upper-left corner of the user dialog "
---

# ToVirtGridCtrl.Right

!!! abstract "Property &middot; `Sudref.chm`"
    Property: Right for XTable

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

Specifies the distance between the right edge of a control and the user dialog box origin. The dialog box origin is in the upper-left corner of the user dialog box.

## Signature

```python
obj.Right
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>If the control is in a tab, the distance is in relation to the upper left corner of the <span class="Monospace">TabPageCtrl</span> control.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
XTable1.Right = 50
```

## See also

<div markdown="1">
<div class="SeeAlso"> </div>
</div>

---

*Source: `Sudref/properties/SUD_property_Right_ToVirtGridCtrl.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*
