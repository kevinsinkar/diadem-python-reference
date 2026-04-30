---
title: "IRepD3PlaneYZInt.Offset"
description: "Specifies the relative displacement of the yz-plane of the 3D axis system along the x-axis in DIAdem REPORT."
---

# IRepD3PlaneYZInt.Offset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Offset for 3DPlaneYZ

Specifies the relative displacement of the yz-plane of the 3D axis system along the x-axis in DIAdem REPORT.

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
oMySettings.PlaneYZ.Offset = -20
oMySettings.PlaneYZ.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Offset_IRepD3PlaneYZInt.htm`*
