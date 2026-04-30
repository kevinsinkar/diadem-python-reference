---
title: "IRepD3AxisSettingsIsometryInt.FitIntoArea"
description: "Specifies whether DIAdem REPORT uses the area spanned by the margins of the 3D axis system completely, or whether DIAdem displays the xy-axes at right angles. I"
---

# IRepD3AxisSettingsIsometryInt.FitIntoArea

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FitIntoArea for 3DAxisSettingsIsometry

Specifies whether DIAdem REPORT uses the area spanned by the margins of the 3D axis system completely, or whether DIAdem displays the xy-axes at right angles. If you do not select this setting, you only can resize the axis system proportionally.

## Signature

```python
obj.FitIntoArea
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
oMyIsometry.Type = dd.e3DAxisIsometryNone
oMyIsometry.FitIntoArea = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FitIntoArea_IRepD3AxisSettingsIsometryInt.htm`*
