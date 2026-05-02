---
title: "IRepTable2DDrawingCellContextInt.RelativeRow"
description: "Specifies the relative row number of the cell that DIAdem is plotting in a 2D table in DIAdem REPORT. The relative row number refers to the row displayed in the"
---

# IRepTable2DDrawingCellContextInt.RelativeRow

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativeRow for 2DTableDrawingCellContext

Specifies the relative row number of the cell that DIAdem is plotting in a 2D table in DIAdem REPORT. The relative row number refers to the row displayed in the table so that the count on the second table page also starts with 1 . If you want to use a row number which corresponds to the data channel, use the property Row for 2DTableDrawingCellContext .

## Signature

```python
obj.RelativeRow
```

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
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn1 = oMy2DTable.Columns.Add(e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
oMy2DTable.Settings.IndexSettings.IndexMode = e2DTableIndexModeAutomaticLastN
oMy2DTable.Settings.IndexSettings.IndexBegin = 20
oMyColumn1.Settings.OnDrawingCell = "MyOnDrawingCell"
```

```python
def MyOnDrawingCell(Context, Cell):
    if (Context.Table.Name == "My2DTable"):
        Cell.Font.Color.SetRGBColor(RGB(255, 128, 128))
        if Context.Row == 1:
            Cell.Value = Cell.Value + " Sheet: " + Context.Sheet.Name
        else:
            Cell.Value = Cell.Value + " Col: " + Context.Col + "; Row: " + Context.Row + "; Rel. row: " + Context.RelativeRow
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativeRow_IRepTable2DDrawingCellContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
