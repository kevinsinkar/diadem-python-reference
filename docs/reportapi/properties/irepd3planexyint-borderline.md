---
title: "IRepD3PlaneXYInt.BorderLine"
description: "Specifies the frame line of the xy plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneXYInt.BorderLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BorderLine for 3DPlaneXY

Specifies the frame line of the xy plane in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.BorderLine
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
oMySettings = oMy3DAxisSystem.Settings
oMySettings.PlaneXY.BorderLine.LineType = dd.eLineTypeDashDot
oMySettings.PlaneXY.BorderLine.Width = dd.eLineWidth0140
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

*Source: `ReportApi/properties/Report_property_BorderLine_IRepD3PlaneXYInt.htm`*
