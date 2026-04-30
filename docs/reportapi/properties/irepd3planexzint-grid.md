---
title: "IRepD3PlaneXZInt.Grid"
description: "Specifies the gridlines of the xz plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneXZInt.Grid

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Grid for 3DPlaneXZ

Specifies the gridlines of the xz plane in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Grid
```

## Python example

```python
dd.Report.NewLayout()
oMy3DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
o3DPlaneXZ = oMy3DaxisSystem.Settings.PlaneXZ
o3DPlaneXZ.Type = dd.e3DPlaneXZTypeXZGrid

o3DPlaneGridXZ = o3DPlaneXZ.Grid
oFullFeaturedLine = o3DPlaneGridXZ.LineX
oFullFeaturedLine.LineType = dd.eLineTypeSolid
oFullFeaturedLine.Color.SetPredefinedColor(dd.eColorIndexRed)

oFullFeaturedLine = o3DPlaneGridXZ.LineZ
oFullFeaturedLine.LineType = dd.eLineTypeSolid
oFullFeaturedLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Grid_IRepD3PlaneXZInt.htm`*
