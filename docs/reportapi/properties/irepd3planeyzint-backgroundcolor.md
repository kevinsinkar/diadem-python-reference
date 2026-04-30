---
title: "IRepD3PlaneYZInt.BackgroundColor"
description: "Specifies the background color of the yz plane in a 3D display in DIAdem REPORT."
---

# IRepD3PlaneYZInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for 3DPlaneYZ

Specifies the background color of the yz plane in a 3D display in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm", "TDM", "")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.PlaneXY.BackgroundColor.SetPredefinedColor(dd.eColorIndexBlue )
oMySettings.PlaneXZ.BackgroundColor.SetPredefinedColor(dd.eColorIndexGreen)
oMySettings.PlaneYZ.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepD3PlaneYZInt.htm`*
