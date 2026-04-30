---
title: "IRepD3AxisSettingsInt.EnableInteractiveRotation"
description: "Specifies in a 3D axis system in DIAdem REPORT whether you can interactively rotate the axis system in the worksheet. If you do not select this setting, you can"
---

# IRepD3AxisSettingsInt.EnableInteractiveRotation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: EnableInteractiveRotation for 3DAxisSettings

Specifies in a 3D axis system in DIAdem REPORT whether you can interactively rotate the axis system in the worksheet. If you do not select this setting, you can only move the axis system in the worksheet.

## Signature

```python
obj.EnableInteractiveRotation
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeMatrix2D, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMySettings.EnableInteractiveRotation = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_EnableInteractiveRotation_IRepD3AxisSettingsInt.htm`*
