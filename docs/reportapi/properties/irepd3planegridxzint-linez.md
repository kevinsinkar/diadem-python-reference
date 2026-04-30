---
title: "IRepD3PlaneGridXZInt.LineZ"
description: "Specifies the properties of the z gridlines in the xz plane of a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneGridXZInt.LineZ

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineZ for 3DPlaneGridXZ

Specifies the properties of the z gridlines in the xz plane of a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.LineZ
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

*Source: `ReportApi/properties/Report_property_LineZ_IRepD3PlaneGridXZInt.htm`*
