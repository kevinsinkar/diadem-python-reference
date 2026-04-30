---
title: "IRepTable2DDrawingHeaderFooterCellInt.BackgroundColor"
description: "Determines the background color of the currently drawn header or footer cell of a 2D table in DIAdem-REPORT within the user command. The user command whose name"
---

# IRepTable2DDrawingHeaderFooterCellInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for 2DTableDrawingHeaderFooterCell

Determines the background color of the currently drawn header or footer cell of a 2D table in DIAdem-REPORT within the user command. The user command whose name is specified in the OnDrawingCell property of the header or footer object is called when the cell is drawn, so that you can change the background color of the cell via the BackgroundColor property depending on a condition.

## Signature

```python
return_value = obj.BackgroundColor
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
    if (Context.TitleNumber = 1):
        if val(Cell.Value) = 0:
            Cell.Font.Color.SetPredefinedColor(ePredefinedColorWhite)
            Cell.BackgroundColor.SetPredefinedColor(ePredefinedColorDarkGreen)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepTable2DDrawingHeaderFooterCellInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
