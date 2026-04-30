---
title: "IRepTable2DDrawingHeaderFooterCellContextInt.TitleNumber"
description: "Determines the number of the currently drawn header or footer cell of a 2D table in DIAdem-REPORT within the user command. Up to three titles can be defined in "
---

# IRepTable2DDrawingHeaderFooterCellContextInt.TitleNumber

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TitleNumber for 2DTableDrawingHeaderFooterCellContext

Determines the number of the currently drawn header or footer cell of a 2D table in DIAdem-REPORT within the user command. Up to three titles can be defined in a table. The object of type 2DTableDrawingHeaderFooterCellContext is passed as the first parameter of the user command. In order for the user command to be called when drawing the header or footer, the name of the function must be set in the OnDrawingCell property of the header or footer object of the table column.

## Signature

```python
obj.TitleNumber
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif" style="width: 26px"/></td><td><strong>Note</strong>  To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
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
    if (Context.TitleNumber = 2):
        if (Context.Col = 1):
            # Show only channel unit and not the value
            Cell.Value = ChnUnit
        else:
            Cell.Value = Cell.Value + " " + ChnUnit
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TitleNumber_IRepTable2DDrawingHeaderFooterCellContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
