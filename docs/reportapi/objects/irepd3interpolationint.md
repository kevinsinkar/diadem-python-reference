---
title: "IRepD3InterpolationInt"
description: "The 3DInterpolation object provides the properties of the curve interpolation in a 3D axis system in the Surface or Characteristic diagram display mode in DIAde"
---

# IRepD3InterpolationInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DInterpolation

The 3DInterpolation object provides the properties of the curve interpolation in a 3D axis system in the Surface or Characteristic diagram display mode in DIAdem REPORT.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3interpolationint-datareductionmode/">DataReductionMode</a> | <a href="../../properties/irepd3interpolationint-datareductionresolution/">DataReductionResolution</a> | <a href="../../properties/irepd3interpolationint-datareductiontype/">DataReductionType</a> | <a href="../../properties/irepd3interpolationint-enable/">Enable</a> | <a href="../../properties/irepd3interpolationint-interpolationmode/">InterpolationMode</a> | <a href="../../properties/irepd3interpolationint-valueredundancymode/">ValueRedundancyMode</a> | <a href="../../properties/irepd3interpolationint-valueredundancytolerance/">ValueRedundancyTolerance</a> | <a href="../../properties/irepd3interpolationint-xbegin/">XBegin</a> | <a href="../../properties/irepd3interpolationint-xend/">XEnd</a> | <a href="../../properties/irepd3interpolationint-xintervalcount/">XIntervalCount</a> | <a href="../../properties/irepd3interpolationint-xmode/">XMode</a> | <a href="../../properties/irepd3interpolationint-ybegin/">YBegin</a> | <a href="../../properties/irepd3interpolationint-yend/">YEnd</a> | <a href="../../properties/irepd3interpolationint-yintervalcount/">YIntervalCount</a> | <a href="../../properties/irepd3interpolationint-ymode/">YMode</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcharacteristicdiagramsettingsint/">3DCharacteristicDiagramSettings</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-interpolation/">Interpolation</a> | <a href="../irepd3shapeobjsurfacesettingsint/">3DSurfaceSettings</a>.<a href="../../properties/irepd3shapeobjsurfacesettingsint-interpolation/">Interpolation</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3InterpolationInt.htm`*
