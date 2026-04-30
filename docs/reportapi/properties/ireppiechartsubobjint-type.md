---
title: "IRepPieChartSubObjInt.Type"
description: "Returns the subobject type of a pie chart in DIAdem REPORT when DIAdem calls the event assigned to the OnPieChart for ToolTipEvents property. DIAdem calls this "
---

# IRepPieChartSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for PieChartSubObj

Returns the subobject type of a pie chart in DIAdem REPORT when DIAdem calls the event assigned to the OnPieChart for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Signature

```python
obj.Type
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartElementMain` | 0 | Main object |
| `ePieChartElementSlice` | 1 | Segment |
| `ePieChartElementLabel` | 2 | Segment label |
| `ePieChartElementLegend` | 3 | Legend |

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
    ToolTipText = "Sheet: " + Context.Sheet.Name + VBCrLf + "-Sub object-" + VBCrLf + "Name: " + oSubObject.Name + VBCrLf + "Index: " + oSubObject.Index + VBCrLf + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + VBCrLf + "X position: " + Context.Position.X + VBCrLf + "Y position: " + Context.Position.Y
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepPieChartSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
