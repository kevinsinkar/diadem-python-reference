---
title: "IRepD3InterpolationInt.InterpolationMode"
description: "Specifies which method DIAdem uses to interpolate the points of a curve interpolation in a 3D axis system with the display type Surface or Characteristic diagra"
---

# IRepD3InterpolationInt.InterpolationMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: InterpolationMode for 3DInterpolation

Specifies which method DIAdem uses to interpolate the points of a curve interpolation in a 3D axis system with the display type Surface or Characteristic diagram in DIAdem REPORT. The two methods differ regarding computing time and results. With the standard number of approximately 50 evaluation points the computing time of both interpolation methods is nearly the same. The computing time of the SCADI increases quadratically with the number of evaluation points and is nearly twice as high as the computing time of the SISPL method when approximately 100 evaluation points are used. In contrast, the computing time of the SISPL method is hardly influenced by the number of evaluation points. If there are many points evenly distributed across the surface, both interpolation methods return nearly identical results. However, if there are only a few points or some values are missing, especially near the edges, the interpolation results differ. The SCADI method extends the existing values at the gaps by continuing the neighboring points’ gradient, whereas the SISPL method extends the existing surface down to the x/y plane to the height of the minimum points. The result of the SISPL resembles an elastic surface which is stretched over the x/y plane and is pulled upwards at the evaluation points. The result of the SCADI resembles a rigid surface which runs through the evaluation points. You can only use the e3DInterpolationModeLinear setting if the TripletStructure for 3DCharacteristicDiagram property contains the e3DCharacteristicTripletStructurePartialLoad value.

## Signature

```python
obj.InterpolationMode
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
oMyInterpolation.YMode = dd.e3DEvaluationPointsNumberManual
oMyInterpolation.XIntervalCount = 30
oMyInterpolation.YIntervalCount = 30
oMyInterpolation.InterpolationMode = dd.e3DInterpolationModeSCADI
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_InterpolationMode_IRepD3InterpolationInt.htm`*
