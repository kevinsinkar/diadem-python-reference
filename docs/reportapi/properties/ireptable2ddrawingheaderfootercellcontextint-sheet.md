---
title: "IRepTable2DDrawingHeaderFooterCellContextInt.Sheet"
description: "Determines the worksheet of the currently drawn cell of a header or footer row in a 2D table in DIAdem-REPORT within the user command. The object of type 2DTabl"
---

# IRepTable2DDrawingHeaderFooterCellContextInt.Sheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sheet for 2DTableDrawingHeaderFooterCellContext

Determines the worksheet of the currently drawn cell of a header or footer row in a 2D table in DIAdem-REPORT within the user command. The object of type 2DTableDrawingHeaderFooterCellContext is passed as the first parameter of the user command. In order for the user command to be called when drawing the header or footer, the name of the function must be set in the OnDrawingCell property of the header or footer object of the table column.

## Signature

```python
return_value = obj.Sheet
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

dd.Report.Sheets.Copy(1, dd.Report.Sheets(1).Name + " green", 2)
```

```python
def OnDrawingFooterCell(Context, Cell):
    if (Context.Sheet.Index == 2) and (Context.TitleNumber == 1):
        Cell.Font.Color.SetPredefinedColor(ePredefinedColorWhite)
        Cell.BackgroundColor.SetPredefinedColor(ePredefinedColorDarkGreen)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Sheet_IRepTable2DDrawingHeaderFooterCellContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
