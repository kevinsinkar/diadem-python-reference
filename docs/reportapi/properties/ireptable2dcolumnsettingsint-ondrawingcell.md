---
title: "IRepTable2DColumnSettingsInt.OnDrawingCell"
description: "Specifies the user command that DIAdem REPORT executes when plotting a curve in a 2D table cell. The user command receives two parameters. The first parameter c"
---

# IRepTable2DColumnSettingsInt.OnDrawingCell

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnDrawingCell for 2DTableColumnSettings

Specifies the user command that DIAdem REPORT executes when plotting a curve in a 2D table cell. The user command receives two parameters. The first parameter corresponds to a 2DTableDrawingCellContext object and provides information about the table, the column, the cell, and the worksheet in which DIAdem is plotting the cell. The second parameter corresponds to a 2DTableDrawingCell object and provides information about the cell DIAdem is plotting. This cell is a temporary copy of the cell defined in the table. You can change this temporary cell any way you like. After plotting this cell, you can no longer access the temporary cell object. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnDrawingCell
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
oMy2DTable.Settings.IndexSettings.IndexMode = e2DTableIndexModeAutomaticallyIncreasing
oMyColumn1.Settings.OnDrawingCell = "MyOnDrawingCell"
```

```python
def MyOnDrawingCell(Context, Cell):
    if (Context.Table.Name = "My2DTable"):
        Cell.Font.Color.SetRGBColor(RGB(255, 128, 128))
        if Context.Row = 1:
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

*Source: `ReportApi/properties/Report_property_OnDrawingCell_IRepTable2DColumnSettingsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
