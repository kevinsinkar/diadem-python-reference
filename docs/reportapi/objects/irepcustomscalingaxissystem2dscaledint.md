---
title: "IRepCustomScalingAxisSystem2DScaledInt"
description: "The AxisSystem2DScaledCustomScaling object provides a user-defined axis scaling in a 2D axis system in DIAdem REPORT in a scaled display."
---

# IRepCustomScalingAxisSystem2DScaledInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AxisSystem2DScaledCustomScaling

The AxisSystem2DScaledCustomScaling object provides a user-defined axis scaling in a 2D axis system in DIAdem REPORT in a scaled display.

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
    if Context.AxisType == e2DAxisTypeY:
        oMyAxis = oMyAxisSystem.YAxisList(Context.AxisNumber)
        MinMax = ValMax(Abs(oMyAxis.Scaling.End),Abs(oMyAxis.Scaling.Begin))
        oMyAxis.Scaling.Origin = oMyAxis.Scaling.Begin
        oMyAxis.Scaling.Begin = -MinMax
        oMyAxis.Scaling.End = +MinMax
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcustomscalingaxissystem2dscaledint-basescalingtype/">BaseScalingType</a> | <a href="../../properties/irepcustomscalingaxissystem2dscaledint-eventname/">EventName</a> | <a href="../../properties/irepcustomscalingaxissystem2dscaledint-id/">ID</a> | <a href="../../properties/irepcustomscalingaxissystem2dscaledint-index/">Index</a> | <a href="../../properties/irepcustomscalingaxissystem2dscaledint-label/">Label</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/axissystem2dscaledcustomscalings/">AxisSystem2DScaledCustomScalings</a>.<a href="../../methods/irepcustomscalingaxissystem2dscaledlistint-add/">Add</a> | <a href="../../collections/axissystem2dscaledcustomscalings/">AxisSystem2DScaledCustomScalings</a>.<a href="../../methods/irepcustomscalingaxissystem2dscaledlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCustomScalingAxisSystem2DScaledInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
