---
title: "IRepTable2DDrawingCellInt"
description: "The 2DTableDrawingCell object provides information about the value cell DIAdem is plotting in a 2D table in DIAdem REPORT."
---

# IRepTable2DDrawingCellInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableDrawingCell

The 2DTableDrawingCell object provides information about the value cell DIAdem is plotting in a 2D table in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2ddrawingcellint-angle/">Angle</a> | <a href="../../properties/ireptable2ddrawingcellint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable2ddrawingcellint-font/">Font</a> | <a href="../../properties/ireptable2ddrawingcellint-value/">Value</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DDrawingCellInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
