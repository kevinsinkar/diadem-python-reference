---
title: "IRepD3ShapeObjIsolinesInt.IsolineType"
description: "Specifies the plane on which DIAdem displays the contour lines of a curve in a 3D axis system in the Isolines display mode in DIAdem REPORT."
---

# IRepD3ShapeObjIsolinesInt.IsolineType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsolineType for 3DIsolines

Specifies the plane on which DIAdem displays the contour lines of a curve in a 3D axis system in the Isolines display mode in DIAdem REPORT.

## Signature

```python
obj.IsolineType
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.IsolineType = dd.e3DIsolineTypeXY
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IsolineType_IRepD3ShapeObjIsolinesInt.htm`*
