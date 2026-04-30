---
title: "IRepD3InterpolationInt.YEnd"
description: "Specifies the maximum grid point in y-direction for the curve interpolation of a 3D axis system in the display modes Surface or Characteristic diagram in DIAdem"
---

# IRepD3InterpolationInt.YEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YEnd for 3DInterpolation

Specifies the maximum grid point in y-direction for the curve interpolation of a 3D axis system in the display modes Surface or Characteristic diagram in DIAdem REPORT, if you assign the value e3DEvaluationPointsManual to the YMode property.

## Signature

```python
obj.YEnd
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

*Source: `ReportApi/properties/Report_property_YEnd_IRepD3InterpolationInt.htm`*
