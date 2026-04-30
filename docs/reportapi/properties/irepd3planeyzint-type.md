---
title: "IRepD3PlaneYZInt.Type"
description: "Specifies whether DIAdem REPORT only displays axes, or if DIAdem also displays frames and grid lines in the yz-plane of the 3D axis system."
---

# IRepD3PlaneYZInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 3DPlaneYZ

Specifies whether DIAdem REPORT only displays axes, or if DIAdem also displays frames and grid lines in the yz-plane of the 3D axis system.

## Signature

```python
obj.Type
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.PlaneXY.Type = dd.e3DPlaneXYTypeNoPlane
oMySettings.PlaneXZ.Type = dd.e3DPlaneXZTypeNoPlane
oMySettings.PlaneYZ.Type = dd.e3DPlaneYZTypeNoPlane
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD3PlaneYZInt.htm`*
