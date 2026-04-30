---
title: "IRepCustomScalingAxisSystem2DScaledListInt.Exists"
description: "Checks whether a user-defined axis scaling with a specific ID already exists in a 2D axis system in DIAdem REPORT in scaled display."
---

# IRepCustomScalingAxisSystem2DScaledListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for AxisSystem2DScaledCustomScalings

Checks whether a user-defined axis scaling with a specific ID already exists in a 2D axis system in DIAdem REPORT in scaled display.

## Signature

```python
bExists = Object.Exists(ID)
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
#Activating Scaled Mode
oDisplayDimensions = dd.Report.Settings.Page.Dimensions
oDisplayDimensions.ScaledHeight = 20
oDisplayDimensions.ScaledWidth = 30
oDisplayDimensions.UseScaledOutput = True
#Creating Axis System and Curve
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 5
oMyPos.X2 = 25
oMyPos.Y1 = 5
oMyPos.Y2 = 15
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DDCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
#Creating Custom Scaling
oMyCustomScalings = dd.Report.Settings.CustomScaling.AxisSystem2DScaledList
if oMyCustomScalings.Exists("MotorWarmScaling") :
    oMyCustomScalings.Remove("MotorWarmScaling")
oMyCustomScalingObj = oMyCustomScalings.Add("MotorWarmScaling")
oMyCustomScalingObj.BaseScalingType = dd.eAxisAutoScalingCompleteAutomatic
oMyCustomScalingObj.EventName = "MyCustomScalingEvent2D"
oMyCustomScalingObj.Label = "LabelForMotorWarmScaling"
#Assigning Custom Scaling to Axis
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingCustom
oMyYScaling.CustomScalingID = "MotorWarmScaling"
dd.Report.Refresh()
```

```python
def MyCustomScalingEvent2D(Context):
    oMyAxisSystem = Context.AxisSystem
    if Context.AxisType == dd.e2DAxisTypeY :
        oMyAxis = oMyAxisSystem.YAxisList(Context.AxisNumber)
        MinMax = dd.ValMax(Abs(oMyAxis.Scaling.End),Abs(oMyAxis.Scaling.Begin))
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

*Source: `ReportApi/methods/Report_method_Exists_IRepCustomScalingAxisSystem2DScaledListInt.htm`*
