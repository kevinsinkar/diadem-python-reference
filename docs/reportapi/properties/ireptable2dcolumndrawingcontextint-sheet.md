---
title: "IRepTable2DColumnDrawingContextInt.Sheet"
description: "Specifies the worksheet of the table column DIAdem is plotting in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnDrawingContextInt.Sheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sheet for 2DTableColumnDrawingContext

Specifies the worksheet of the table column DIAdem is plotting in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Sheet
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
AddUserCommandToEvent("dd.Report.Events.OnDrawing2DTableColumn", "MMyOnDrawing2DTableColumn")

def MyOnDrawing2DTableColumn(Context, Column):
    oMyTable = Context.Table
    oMyColumn = Column
    if Context.Sheet.Index = 1 AND oMyTable.Index = 1:
        # select oMyColumn.Type
        # case e2DTableColumnChannel
        oMyColumn.Settings.Format = "d.d"
        # case e2DTableColumnVariable
        # case e2DTableColumnExpression
        # case e2DTableColumnText
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Sheet_IRepTable2DColumnDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
