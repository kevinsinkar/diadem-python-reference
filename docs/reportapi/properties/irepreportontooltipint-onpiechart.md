---
title: "IRepReportOnToolTipInt.OnPieChart"
description: "Specifies the user command which DIAdem REPORT executes when you press the shift key and move the mouse over a pie chart. The user command receives two paramete"
---

# IRepReportOnToolTipInt.OnPieChart

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnPieChart for ToolTipEvents

Specifies the user command which DIAdem REPORT executes when you press the shift key and move the mouse over a pie chart. The user command receives two parameters. The first parameter corresponds to a ToolTipPieChartContext object and provides information about the pie chart in DIAdem REPORT. The second parameter is a text and is the same as displayed on the tooltip.

## Signature

```python
obj.OnPieChart
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
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMyPieChart = dd.Report.ActiveSheet.Objects.Add(eReportObjectPieChart, "MyPieChart")
oMyPos = oMyPieChart.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurvePieChart = oMyPieChart.CurvePieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
oMySliceLabel = oMyCurvePieChart.SliceLabel
oMySliceLabel.CategoryVisible = True
oMySliceLabel.Channel.Reference = "[5]/[1]"
oMySliceLabel.CategoryMode = eCategoryModeChannel
# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnPieChart = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "-Sub object-" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Index: " + oSubObject.Index + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + "\r\n" + "X position: " + Context.Position.X + "\r\n" + "Y position: " + Context.Position.Y
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnPieChart_IRepReportOnToolTipInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
