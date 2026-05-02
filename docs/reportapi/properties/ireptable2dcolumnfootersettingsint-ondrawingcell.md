---
title: "IRepTable2DColumnFooterSettingsInt.OnDrawingCell"
description: "Specifies the user command that DIAdem REPORT executes when drawing the footer of a 2D table column. The event starts the user command that you assigned to the "
---

# IRepTable2DColumnFooterSettingsInt.OnDrawingCell

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnDrawingCell for 2DTableColumnFooterSettings

Specifies the user command that DIAdem REPORT executes when drawing the footer of a 2D table column. The event starts the user command that you assigned to the OnDrawingCell property. The user command receives two parameters. The first parameter corresponds to a 2DTableDrawingHeaderFooterCellContext object and provides information about the table, the column, the footer, and the worksheet in which DIAdem is plotting the footer. The second parameter corresponds to a 2DTableDrawingHeaderFooterCell object and provides information about the cell DIAdem is plotting. This cell is a temporary copy of the cell defined in the table. You can change this temporary cell any way you like. After plotting this cell, you can no longer access the temporary cell object. DIAdem REPORT saves this property in the layout.

## Signature

```python
obj.OnDrawingCell
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
Table = dd.Report.ActiveSheet.Objects.Add(eReportObject2DTable, "2DTableFooter")
Position = Table.Position.ByBorder
Position.Top = 20
Position.Bottom = 20
Position.Left = 20
Position.Right = 30

Table.Settings.Footer.Visible = true
Table.Settings.Footer.Height = 12
Table.Settings.Footer.TitleDefinition1 = e2DTableTitleChnMinAll
Table.Settings.Footer.TitleDefinition2 = e2DTableTitleChnMaxAll

Column = Table.Columns.Add(e2DTableColumnChannel)
Column.Channel.Reference = "[1]/[1]"
Column.Settings.Footer.OnDrawingCell = "OnDrawingFooterCell"

Column = Table.Columns.Add(e2DTableColumnChannel)
Column.Channel.Reference = "[1]/[2]"
Column.Settings.Footer.OnDrawingCell = "OnDrawingFooterCell"
```

```python
def OnDrawingFooterCell(Context, Cell):
    if (Context.TitleNumber == 1):
        if val(Cell.Value) == 0:
            Cell.Font.Color.SetPredefinedColor(ePredefinedColorWhite)
            Cell.BackgroundColor.SetPredefinedColor(ePredefinedColorDarkGreen)
        Cell.Value = "Min: " + Cell.Value
    if (Context.Col == 2) and (Context.TitleNumber == 2):
        Cell.Value = Cell.Value + " " + ChnUnit
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnDrawingCell_IRepTable2DColumnFooterSettingsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
