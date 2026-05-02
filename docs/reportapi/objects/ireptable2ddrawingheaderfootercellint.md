---
title: "IRepTable2DDrawingHeaderFooterCellInt"
description: "The 2DTableDrawingHeaderFooterCell object provides information within the user command about the cell of a header or footer of the 2D table that is currently be"
---

# IRepTable2DDrawingHeaderFooterCellInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableDrawingHeaderFooterCell

The 2DTableDrawingHeaderFooterCell object provides information within the user command about the cell of a header or footer of the 2D table that is currently being drawn in DIAdem-REPORT. The current content and the appearance of the header or footer can be determined and changed via the properties of the object. The user command whose name is specified in the OnDrawingCell property of the header or footer object is called when the cell is drawn. The second parameter corresponds to the 2DTableDrawingHeaderFooter Cell object. This cell is a temporary copy of the cell defined in the table. You can change this temporary cell any way you like. After plotting this cell, you can no longer access the temporary cell object.

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
                Cell.BackgroundColor.SetRGBColor(RGB(255, 128, 128))
                Cell.Font.Color.SetPredefinedColor(ePredefinedColorWhite)
            Cell.Value = Cell.Value + " " + ChnUnit
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2ddrawingheaderfootercellint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable2ddrawingheaderfootercellint-font/">Font</a> | <a href="../../properties/ireptable2ddrawingheaderfootercellint-value/">Value</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DDrawingHeaderFooterCellInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
