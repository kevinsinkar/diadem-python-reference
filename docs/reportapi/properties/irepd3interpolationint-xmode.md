---
title: "IRepD3InterpolationInt.XMode"
description: "Specifies how DIAdem REPORT specifies the origin of the grid points in x-direction for the curve interpolation of a 3D axis system in the display modes Surface "
---

# IRepD3InterpolationInt.XMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XMode for 3DInterpolation

Specifies how DIAdem REPORT specifies the origin of the grid points in x-direction for the curve interpolation of a 3D axis system in the display modes Surface or Characteristic diagram .

## Signature

```python
obj.XMode
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue )
oMyInterpolation = oMySettings.Interpolation
oMyInterpolation.Enable = True
oMyInterpolation.XMode = dd.e3DEvaluationPointsManual
oMyInterpolation.YMode = dd.e3DEvaluationPointsManual
oMyInterpolation.XIntervalCount = 100
oMyInterpolation.YIntervalCount = 100
oMyInterpolation.XBegin = 0
oMyInterpolation.XEnd = 1
oMyInterpolation.YBegin = 0
oMyInterpolation.YEnd = 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XMode_IRepD3InterpolationInt.htm`*
