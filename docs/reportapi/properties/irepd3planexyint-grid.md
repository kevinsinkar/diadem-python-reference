---
title: "IRepD3PlaneXYInt.Grid"
description: "Specifies the gridlines of the xy plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneXYInt.Grid

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Grid for 3DPlaneXY

Specifies the gridlines of the xy plane in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Grid
```

## Python example

```python
dd.Report.NewLayout()
oMy3DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
o3DPlaneXY = oMy3DaxisSystem.Settings.PlaneXY
o3DPlaneXY.Type = dd.e3DPlaneXYTypeXYGrid

o3DPlaneGridXY = o3DPlaneXY.Grid
oFullFeaturedLine = o3DPlaneGridXZ.LineX
oFullFeaturedLine.LineType = dd.eLineTypeSolid
oFullFeaturedLine.Color.SetPredefinedColor(dd.eColorIndexRed)

oFullFeaturedLine = o3DPlaneGridXZ.LineY
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

*Source: `ReportApi/properties/Report_property_Grid_IRepD3PlaneXYInt.htm`*
