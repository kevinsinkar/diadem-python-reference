---
title: "IRepCustomScalingAxisSystem2DContextInt"
description: "The CustomScalingAxisSystem2DContext object provides information about the worksheet, the axis system, and the ID for a user-defined axis scaling in a 2D axis s"
---

# IRepCustomScalingAxisSystem2DContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CustomScalingAxisSystem2DContext

The CustomScalingAxisSystem2DContext object provides information about the worksheet, the axis system, and the ID for a user-defined axis scaling in a 2D axis system in DIAdem REPORT.

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
# Creating Axis System and Curve
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(e2DShapeLine, "My2DDCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
# Creating Custom Scaling
oMyCustomScalings = dd.Report.Settings.CustomScaling.AxisSystem2DList
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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcustomscalingaxissystem2dcontextint-axisnumber/">AxisNumber</a> | <a href="../../properties/irepcustomscalingaxissystem2dcontextint-axissystem/">AxisSystem</a> | <a href="../../properties/irepcustomscalingaxissystem2dcontextint-axistype/">AxisType</a> | <a href="../../properties/irepcustomscalingaxissystem2dcontextint-customscalingid/">CustomScalingID</a> | <a href="../../properties/irepcustomscalingaxissystem2dcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCustomScalingAxisSystem2DContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
