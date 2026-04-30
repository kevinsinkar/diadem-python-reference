---
title: "IRepCustomScalingSettingsInt.AxisSystem3DList"
description: "Specifies user-defined axis scalings in a 3D axis system in DIAdem REPORT."
---

# IRepCustomScalingSettingsInt.AxisSystem3DList

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisSystem3DList for CustomScaling

Specifies user-defined axis scalings in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.AxisSystem3DList
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
#Creating Axis System and Curve
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DaxisSystem.Curves3D.Add(dd.e3DShapeSurface, "My3DDCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
#Creating Custom Scaling
oMyCustomScalings = dd.Report.Settings.CustomScaling.AxisSystem3DList
oMyCustomScalings.RemoveAll()
oMyCustomScalingObj = oMyCustomScalings.Add("MotorWarmScaling")
oMyCustomScalingObj.BaseScalingType = dd.eAxisAutoScalingCompleteAutomatic
oMyCustomScalingObj.EventName = "MyCustomScalingEvent3D"
oMyCustomScalingObj.Label = "LabelForMotorWarmScaling"
#Assigning Custom Scaling to Axis
oMyYScaling = oMy3DAxisSystem.AxisList.Y.Scaling
oMyYScaling.AutoScalingType = dd.eAxisScalingSimpleCustom
oMyYScaling.CustomScalingID = "MotorWarmScaling"
dd.Report.Refresh()
```

```python
def MyCustomScalingEvent3D(Context):
    oMyAxisSystem = Context.AxisSystem
    select_variable_0 = Context.AxisType
    if (select_variable_0 == dd.e3DAxisTypeX) :
        oMyAxis = oMyAxisSystem.AxisList.X
    elif (select_variable_0 == dd.e3DAxisTypeY) :
        oMyAxis = oMyAxisSystem.AxisList.Y
    elif (select_variable_0 == dd.e3DAxisTypeZ) :
        oMyAxis = oMyAxisSystem.AxisList.Z
    else:
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

*Source: `ReportApi/properties/Report_property_AxisSystem3DList_IRepCustomScalingSettingsInt.htm`*
