---
title: "IRepCustomScalingAxisSystem2DScaledInt.ID"
description: "Specifies the ID of a user-defined scaling in a 2D axis system in DIAdem REPORT in a scaled display. The ID links the axis to a user-defined scaling."
---

# IRepCustomScalingAxisSystem2DScaledInt.ID

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ID for AxisSystem2DScaledCustomScaling

Specifies the ID of a user-defined scaling in a 2D axis system in DIAdem REPORT in a scaled display. The ID links the axis to a user-defined scaling.

## Signature

```python
obj.ID
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong> To test the following example scripts, first save the bottom script and select <strong>Settings»Extensions»User Commands</strong> to register it as a user command.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Example.tdm","TDM","")
# Activating Scaled Mode
oDisplayDimensions = dd.Report.Settings.Page.Dimensions
oDisplayDimensions.ScaledHeight = 20
oDisplayDimensions.ScaledWidth = 30
oDisplayDimensions.UseScaledOutput = True
# Creating Axis System and Curve
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 5
oMyPos.X2 = 25
oMyPos.Y1 = 5
oMyPos.Y2 = 15
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(e2DShapeLine, "My2DDCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
# Creating Custom Scaling
oMyCustomScalings = dd.Report.Settings.CustomScaling.AxisSystem2DScaledList
MsgBoxDisp("ID: "& oMyCustomScalings.Item(1).ID)
oMyCustomScalings.RemoveAll
oMyCustomScalingObj = oMyCustomScalings.Add("MotorWarmScaling")
oMyCustomScalingObj.BaseScalingType = eAxisAutoScalingCompleteAutomatic
oMyCustomScalingObj.EventName = "MyCustomScalingEvent2D"
oMyCustomScalingObj.Label = "LabelForMotorWarmScaling"
# Assigning Custom Scaling to Axis
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = eAxisAutoScalingCustom
oMyYScaling.CustomScalingID = "MotorWarmScaling"
dd.Report.Refresh()
```

```python
def MyCustomScalingEvent2D(Context):
    oMyAxisSystem = Context.AxisSystem
    if Context.AxisType = e2DAxisTypeY:
        oMyAxis = oMyAxisSystem.YAxisList(Context.AxisNumber)
        MinMax = ValMax(Abs(oMyAxis.Scaling.End),Abs(oMyAxis.Scaling.Begin))
        oMyAxis.Scaling.Origin = oMyAxis.Scaling.Begin
        oMyAxis.Scaling.Begin = -MinMax
        oMyAxis.Scaling.End = +MinMax
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ID_IRepCustomScalingAxisSystem2DScaledInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
