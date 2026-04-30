---
title: "IRepD3PlaneGridYZInt"
description: "The 3DPlaneGridYZ object provides the properties of the gridlines of the yz-plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneGridYZInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DPlaneGridYZ

The 3DPlaneGridYZ object provides the properties of the gridlines of the yz-plane in a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy3DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
o3DPlaneYZ = oMy3DaxisSystem.Settings.PlaneYZ
o3DPlaneYZ.Type = dd.e3DPlaneYZTypeYZGrid

o3DPlaneGridYZ = o3DPlaneYZ.Grid
oFullFeaturedLine = o3DPlaneGridYZ.LineY
oFullFeaturedLine.LineType = dd.eLineTypeSolid
oFullFeaturedLine.Color.SetPredefinedColor(dd.eColorIndexRed)

oFullFeaturedLine = o3DPlaneGridYZ.LineZ
oFullFeaturedLine.LineType = dd.eLineTypeSolid
oFullFeaturedLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3planegridyzint-liney/">LineY</a> | <a href="../../properties/irepd3planegridyzint-linez/">LineZ</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3planeyzint/">3DPlaneYZ</a>.<a href="../../properties/irepd3planeyzint-grid/">Grid</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3PlaneGridYZInt.htm`*
