---
title: "IRepTable2DDrawingHeaderFooterCellContextInt"
description: "The 2DTableDrawingHeaderFooterCellContext object provides information within the user command about the 2D table whose header or footer is currently being drawn"
---

# IRepTable2DDrawingHeaderFooterCellContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableDrawingHeaderFooterCellContext

The 2DTableDrawingHeaderFooterCellContext object provides information within the user command about the 2D table whose header or footer is currently being drawn in DIAdem-REPORT. This object is passed as the first parameter of the user command. In order for the user command to be called when drawing the header or footer, the name of the function must be set in the OnDrawingCell property of the header or footer object of the table column.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
Table = dd.Report.ActiveSheet.Objects.Add(eReportObject2DTable, "2DTableUnitTitle")
Position = Table.Position.ByBorder
Position.Top = 20
Position.Bottom = 20
Position.Left = 20
Position.Right = 30

Table.Settings.Header.Height = 15
Table.Settings.Header.TitleDefinition1 = e2DTableTitleChnName
Table.Settings.Header.TitleDefinition2 = e2DTableTitleChnMaxAll

Column = Table.Columns.Add(e2DTableColumnChannel)
Column.Channel.Reference = "[1]/[1]"
Column.Settings.Header.OnDrawingCell = "OnDrawingHeaderCell"

Column = Table.Columns.Add(e2DTableColumnChannel)
Column.Channel.Reference = "[1]/[2]"
Column.Settings.Header.OnDrawingCell = "OnDrawingHeaderCell"
```

```python
def OnDrawingHeaderCell(Context, Cell):
    if (Context.TitleNumber == 2):
        if (Context.Col == 1):
            # Show only channel unit
            Cell.Value = ChnUnit
        else:
            # Maximum (in red) with channel unit
            if val(Cell.Value) > 0:
                Cell.Font.Color.SetRGBColor(dd.RGB(255, 128, 128))
            Cell.Value = Cell.Value + " " + ChnUnit
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/ireptable2ddrawingheaderfootercellcontextint-col/">Col</a> | <a href="../../properties/ireptable2ddrawingheaderfootercellcontextint-sheet/">Sheet</a> | <a href="../../properties/ireptable2ddrawingheaderfootercellcontextint-table/">Table</a> | <a href="../../properties/ireptable2ddrawingheaderfootercellcontextint-titlenumber/">TitleNumber</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DDrawingHeaderFooterCellContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
