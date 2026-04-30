---
title: "IRepD3InterpolationInt.ValueRedundancyTolerance"
description: "Specifies the tolerance as a percentage of the total x-area and y-area within which DIAdem REPORT combines the x- and y-value pairs to one value pair when inter"
---

# IRepD3InterpolationInt.ValueRedundancyTolerance

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueRedundancyTolerance for 3DInterpolation

Specifies the tolerance as a percentage of the total x-area and y-area within which DIAdem REPORT combines the x- and y-value pairs to one value pair when interpolating a surface.

## Signature

```python
obj.ValueRedundancyTolerance
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

*Source: `ReportApi/properties/Report_property_ValueRedundancyTolerance_IRepD3InterpolationInt.htm`*
