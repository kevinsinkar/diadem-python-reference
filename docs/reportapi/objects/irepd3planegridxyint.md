---
title: "IRepD3PlaneGridXYInt"
description: "The 3DPlaneGridXY object provides the properties of the gridlines of the xy-plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneGridXYInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DPlaneGridXY

The 3DPlaneGridXY object provides the properties of the gridlines of the xy-plane in a 3D axis system in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3planegridxyint-linex/">LineX</a> | <a href="../../properties/irepd3planegridxyint-liney/">LineY</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3planexyint/">3DPlaneXY</a>.<a href="../../properties/irepd3planexyint-grid/">Grid</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3PlaneGridXYInt.htm`*
