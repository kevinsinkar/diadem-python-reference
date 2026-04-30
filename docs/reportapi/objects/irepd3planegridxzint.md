---
title: "IRepD3PlaneGridXZInt"
description: "The 3DPlaneGridXZ object provides the properties of the gridlines of the xz-plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneGridXZInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DPlaneGridXZ

The 3DPlaneGridXZ object provides the properties of the gridlines of the xz-plane in a 3D axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepd3planegridxzint-linex/">LineX</a> | <a href="../../properties/irepd3planegridxzint-linez/">LineZ</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3planexzint/">3DPlaneXZ</a>.<a href="../../properties/irepd3planexzint-grid/">Grid</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3PlaneGridXZInt.htm`*
