---
title: "IRepTable2DDrawingHeaderFooterCellInt.Value"
description: "Determines the value of the currently drawn header or footer cell of a 2D table in DIAdem-REPORT within the user command. The user command, whose name is specif"
---

# IRepTable2DDrawingHeaderFooterCellInt.Value

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Value for 2DTableDrawingHeaderFooterCell

Determines the value of the currently drawn header or footer cell of a 2D table in DIAdem-REPORT within the user command. The user command, whose name is specified in the OnDrawingCell property of the header or footer object , is called when the cell is drawn so that you can change the content of the cell as required using the Value property.

## Signature

```python
obj.Value
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
                Cell.Font.Color.SetRGBColor(RGB(255, 128, 128))
            Cell.Value = Cell.Value + " " + ChnUnit
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Value_IRepTable2DDrawingHeaderFooterCellInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
