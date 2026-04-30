---
title: "IRepD3PlaneYZInt.Grid"
description: "Specifies the gridlines of the yz plane in a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneYZInt.Grid

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Grid for 3DPlaneYZ

Specifies the gridlines of the yz plane in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Grid
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Grid_IRepD3PlaneYZInt.htm`*
