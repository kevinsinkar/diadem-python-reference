---
title: "IRepTable2DDropContextInt.ColumnIndex"
description: "Specifies the index of the column in a 2D table onto which you dragged and dropped an object."
---

# IRepTable2DDropContextInt.ColumnIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColumnIndex for 2DTableDropContext

Specifies the index of the column in a 2D table onto which you dragged and dropped an object.

## Signature

```python
obj.ColumnIndex
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Report.Events.OnDrop2DTable", "MyOnDrop2DTableEvent")

def MyOnDrop2DTableEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + "\r\n" + oMyDropElement.Name
    Msgbox(sOutput)
    oMyTable = Context.Table
    if Context.ColumnIndex>0:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyTable.Name + "\r\n" + oMyTable.Columns.Item(Context.ColumnIndex).Type)
    else:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyTable.Name)
    Context.DoProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColumnIndex_IRepTable2DDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
