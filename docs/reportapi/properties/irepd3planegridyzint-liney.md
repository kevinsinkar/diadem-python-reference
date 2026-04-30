---
title: "IRepD3PlaneGridYZInt.LineY"
description: "Specifies the properties of the y gridlines in the yz plane of a 3D axis system in DIAdem REPORT."
---

# IRepD3PlaneGridYZInt.LineY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineY for 3DPlaneGridYZ

Specifies the properties of the y gridlines in the yz plane of a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.LineY
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

*Source: `ReportApi/properties/Report_property_LineY_IRepD3PlaneGridYZInt.htm`*
