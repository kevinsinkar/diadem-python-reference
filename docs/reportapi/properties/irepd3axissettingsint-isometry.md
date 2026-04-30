---
title: "IRepD3AxisSettingsInt.Isometry"
description: "Specifies the properties of the isometric axis adaptation in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisSettingsInt.Isometry

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Isometry for 3DAxisSettings

Specifies the properties of the isometric axis adaptation in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Isometry
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMyIsometry = oMy3DAxisSystem.Settings.Isometry
oMyIsometry.Type = dd.e3DAxisIsometryXY
oMyIsometry.Length = 50
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Isometry_IRepD3AxisSettingsInt.htm`*
