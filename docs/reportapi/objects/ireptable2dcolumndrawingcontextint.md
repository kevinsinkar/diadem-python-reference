---
title: "IRepTable2DColumnDrawingContextInt"
description: "The 2DTableColumnDrawingContext object provides information about the 2D table and the worksheet into which DIAdem REPORT is plotting the table column. The obje"
---

# IRepTable2DColumnDrawingContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnDrawingContext

The 2DTableColumnDrawingContext object provides information about the 2D table and the worksheet into which DIAdem REPORT is plotting the table column. The object corresponds with the first parameter of the user command , which you assigned to the property Report.Events. OnCurveTransformation .

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
    if Context.Sheet.Index = 1 AND oMyTable.Index = 1:
        # select oMyColumn.Type
        # case e2DTableColumnChannel
        oMyColumn.Settings.Format = "d.d"
        # case e2DTableColumnVariable
        # case e2DTableColumnExpression
        # case e2DTableColumnText
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumndrawingcontextint-sheet/">Sheet</a> | <a href="../../properties/ireptable2dcolumndrawingcontextint-table/">Table</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
