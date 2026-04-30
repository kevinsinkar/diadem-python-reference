---
title: "IRepD3PlaneGridXYInt.LineY"
description: "Specifies the properties of the y gridlines in the xy plane of a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneGridXYInt.LineY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineY for 3DPlaneGridXY

Specifies the properties of the y gridlines in the xy plane of a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.LineY
```

## Python example

```python
dd.Report.NewLayout()
oMy3DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
o3DPlaneXY = oMy3DaxisSystem.Settings.PlaneXY
o3DPlaneXY.Type = dd.e3DPlaneXYTypeXYGrid

o3DPlaneGridXY = o3DPlaneXY.Grid
oFullFeaturedLine = o3DPlaneGridXY.LineX
oFullFeaturedLine.LineType = dd.eLineTypeSolid
oFullFeaturedLine.Color.SetPredefinedColor(dd.eColorIndexRed)

oFullFeaturedLine = o3DPlaneGridXY.LineY
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

*Source: `ReportApi/properties/Report_property_LineY_IRepD3PlaneGridXYInt.htm`*
