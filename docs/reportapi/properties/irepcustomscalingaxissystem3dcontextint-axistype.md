---
title: "IRepCustomScalingAxisSystem3DContextInt.AxisType"
description: "Specifies in a 3D axis system in DIAdem REPORT the type of axis to which you assign a user-defined axis scaling."
---

# IRepCustomScalingAxisSystem3DContextInt.AxisType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisType for CustomScalingAxisSystem3DContext

Specifies in a 3D axis system in DIAdem REPORT the type of axis to which you assign a user-defined axis scaling.

## Signature

```python
obj.AxisType
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
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")
# Creating Axis System and Curve
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DaxisSystem.Curves3D.Add(e3DShapeSurface, "My3DDCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
# Creating Custom Scaling
oMyCustomScalings = dd.Report.Settings.CustomScaling.AxisSystem3DList
oMyCustomScalings.RemoveAll()
oMyCustomScalingObj = oMyCustomScalings.Add("MotorWarmScaling")
oMyCustomScalingObj.BaseScalingType = eAxisAutoScalingCompleteAutomatic
oMyCustomScalingObj.EventName = "MyCustomScalingEvent3D"
oMyCustomScalingObj.Label = "LabelForMotorWarmScaling"
# Assigning Custom Scaling to Axis
oMyYScaling = oMy3DAxisSystem.AxisList.Y.Scaling
oMyYScaling.AutoScalingType = eAxisScalingSimpleCustom
oMyYScaling.CustomScalingID = "MotorWarmScaling"
dd.Report.Refresh()
```

```python
def MyCustomScalingEvent3D(Context):
    oMyAxisSystem = Context.AxisSystem
    # select Context.AxisType
    # case e3DAxisTypeX
    oMyAxis = oMyAxisSystem.AxisList.X
    # case e3DAxisTypeY
    oMyAxis = oMyAxisSystem.AxisList.Y
    # case e3DAxisTypeZ
    oMyAxis = oMyAxisSystem.AxisList.Z
    # case else
    return
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

*Source: `ReportApi/properties/Report_property_AxisType_IRepCustomScalingAxisSystem3DContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
