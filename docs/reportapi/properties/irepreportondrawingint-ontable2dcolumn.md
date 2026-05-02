---
title: "IRepReportOnDrawingInt.OnTable2DColumn"
description: "Specifies the user command that DIAdem REPORT executes when plotting a curve in a 2D table column. The user command receives two parameters. The first parameter"
---

# IRepReportOnDrawingInt.OnTable2DColumn

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnTable2DColumn for DrawingEvents

Specifies the user command that DIAdem REPORT executes when plotting a curve in a 2D table column. The user command receives two parameters. The first parameter corresponds to a 2DTableColumnDrawingContext object and provides information about the 2D table and the worksheet into which DIAdem is plotting the curve. The second parameter corresponds to a 2DTableColumn object and provides information about the table column DIAdem is plotting. This table column is a temporary copy of the table column defined in the table. You can change this temporary table column any way you like. After plotting this table column, you can no longer access the temporary 2DTableColumn object. DIAdem REPORT saves this property with the layout. The user command is only executed if you use the Enable for CurveExpansionSettings property to enable the expansion mode.

## Signature

```python
obj.OnTable2DColumn
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.Drawing.OnTable2DColumn = "MyOnDrawing2DTableColumn"

def MyOnDrawing2DTableColumn(Context, Column):
    oMyTable = Context.Table
    oMyColumn = Column
    if Context.Sheet.Index == 1 AND oMyTable.Index == 1:
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

*Source: `ReportApi/properties/Report_property_OnTable2DColumn_IRepReportOnDrawingInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
