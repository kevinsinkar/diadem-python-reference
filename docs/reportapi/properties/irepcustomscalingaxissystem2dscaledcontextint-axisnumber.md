---
title: "IRepCustomScalingAxisSystem2DScaledContextInt.AxisNumber"
description: "Specifies in a 2D axis system in scaled display in DIAdem REPORT the number of the axis to which you assign a user-defined scaling."
---

# IRepCustomScalingAxisSystem2DScaledContextInt.AxisNumber

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisNumber for CustomScalingAxisSystem2DScaledContext

Specifies in a 2D axis system in scaled display in DIAdem REPORT the number of the axis to which you assign a user-defined scaling.

## Signature

```python
obj.AxisNumber
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
# Creating axis system
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 5
oMyPos.X2 = 25
oMyPos.Y1 = 5
oMyPos.Y2 = 15
# Creating secondary y axis
oMySecondAxis = oMy2DaxisSystem.YAxisList.Add("SecondAxis")
# Creating curves and assigning axes
oMy2DCurve1 = oMy2DAxisSystem.Curves2D.Add(e2DShapeLine, "My2DCurve1")
oMy2DCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve1.YAxisReference = oMy2DAxisSystem.YAxisList(1).Name
oMy2DCurve2 = oMy2DAxisSystem.Curves2D.Add(e2DShapeLine, "My2DCurve2")
oMy2DCurve2.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[3]"
oMy2DCurve2.YAxisReference = "SecondAxis"  # or oMySecondAxis.Name
# Creating custom scaling
oMyCustomScalings = dd.Report.Settings.CustomScaling.AxisSystem2DScaledList
oMyCustomScalings.RemoveAll
oMyCustomScalingObj = oMyCustomScalings.Add("MotorWarmScaling")
oMyCustomScalingObj.BaseScalingType = eAxisAutoScalingCompleteAutomatic
oMyCustomScalingObj.EventName = "MyCustomScalingEvent2D"
oMyCustomScalingObj.Label = "LabelForMotorWarmScaling"
# Assigning custom scaling to first axis
oMyYScaling1 = oMy2DAxisSystem.YAxisList(1).Scaling
oMyYScaling1.AutoScalingType = eAxisAutoScalingCustom
oMyYScaling1.CustomScalingID = "MotorWarmScaling"
# Assigning custom scaling to second axis
oMyYScaling2 = oMy2DAxisSystem.YAxisList(2).Scaling
oMyYScaling2.AutoScalingType = eAxisAutoScalingCustom
oMyYScaling2.CustomScalingID = "MotorWarmScaling"
dd.Report.Refresh()
```

```python
def MyCustomScalingEvent2D(Context):
    oMyAxisSystem = Context.AxisSystem
    if Context.AxisType == e2DAxisTypeY:
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

*Source: `ReportApi/properties/Report_property_AxisNumber_IRepCustomScalingAxisSystem2DScaledContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
