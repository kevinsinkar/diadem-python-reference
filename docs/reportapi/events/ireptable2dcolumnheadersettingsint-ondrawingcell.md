---
title: "IRepTable2DColumnHeaderSettingsInt.OnDrawingCell"
description: "Is triggered in DIAdem-REPORT while drawing the header of a 2D table column. The event starts the user command that you assigned to the property OnDrawingCell f"
---

# IRepTable2DColumnHeaderSettingsInt.OnDrawingCell

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnDrawingCell for 2DTableColumnHeaderSettings

Is triggered in DIAdem-REPORT while drawing the header of a 2D table column. The event starts the user command that you assigned to the property OnDrawingCell for 2DTableColumnHeaderSettings . The user command receives two parameters. The first parameter corresponds to a 2DTableDrawingHeaderFooterCellContext object and provides information about the table, the column, the header, and the worksheet in which DIAdem is plotting the header. The second parameter corresponds to a 2DTableDrawingHeaderFooterCell object and provides information about the cell DIAdem is plotting. This cell is a temporary copy of the cell defined in the table. You can change this temporary cell any way you like. After plotting this cell, you can no longer access the temporary cell object. Refer to Working with Events in DIAdem for more information on events in DIAdem.

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnDrawingCell_IRepTable2DColumnHeaderSettingsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
