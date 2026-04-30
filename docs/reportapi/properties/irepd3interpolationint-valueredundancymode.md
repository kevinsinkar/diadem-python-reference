---
title: "IRepD3InterpolationInt.ValueRedundancyMode"
description: "Specifies how DIAdem combines triplet points whose x-values and y-values are close to each other, in a surface interpolation. If the data is in a triplet struct"
---

# IRepD3InterpolationInt.ValueRedundancyMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueRedundancyMode for 3DInterpolation

Specifies how DIAdem combines triplet points whose x-values and y-values are close to each other, in a surface interpolation. If the data is in a triplet structure, the x-values and y-values are grouped into new x-channels and y-channels respectively, and the z-values are saved as a matrix. During data acquisition several quasi identical (x,y)-points might have been acquired. Therefore you must specify a tolerance when you convert data so that values which deviate due to measurement inaccuracies are saved only once in the matrix. You can select whether DIAdem uses the lowest, the highest, or the average value, whether DIAdem uses the first or the last value in a channel list, or whether DIAdem summates all values within the specified tolerance.

## Signature

```python
obj.ValueRedundancyMode
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
oMyInterpolation.YMode = dd.e3DEvaluationPointsManual
oMyInterpolation.XIntervalCount = 30
oMyInterpolation.YIntervalCount = 30
oMyInterpolation.ValueRedundancyMode = dd.e3DRedundancyMeanValue
oMyInterpolation.ValueRedundancyTolerance = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ValueRedundancyMode_IRepD3InterpolationInt.htm`*
