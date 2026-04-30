---
title: "IRepD3ShapeObj2DMatrixInt.XChannel"
description: "Specifies the x-channel of a curve in the 2D matrix display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObj2DMatrixInt.XChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XChannel for 3DMatrix2D

Specifies the x-channel of a curve in the 2D matrix display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.XChannel
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeMatrix2D, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XChannel_IRepD3ShapeObj2DMatrixInt.htm`*
