---
title: "IRepD3MarkerAdditionalInt.Size"
description: "Specifies the marker size in a 3D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for 3DAdditionalMarker

Specifies the marker size in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Size
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapePoints, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.Settings.Marker.Type = dd.eMarkerAsterisk
oMyShape.Settings.Marker.Size = 1.4
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepD3MarkerAdditionalInt.htm`*
