---
title: "IRepD3PlaneXYInt.Offset"
description: "Specifies the relative displacement of the xy-plane of the 3D axis system along the z-axis in DIAdem REPORT."
---

# IRepD3PlaneXYInt.Offset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Offset for 3DPlaneXY

Specifies the relative displacement of the xy-plane of the 3D axis system along the z-axis in DIAdem REPORT.

## Signature

```python
obj.Offset
```

## Python example

```python
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy3DAxisSystem.Settings
oMySettings.PlaneXY.Offset = -20
oMySettings.PlaneXY.BackgroundColor.SetPredefinedColor(dd.eColorIndexBlue )
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Offset_IRepD3PlaneXYInt.htm`*
