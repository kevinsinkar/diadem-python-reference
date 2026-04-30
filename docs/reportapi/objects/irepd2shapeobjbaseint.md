---
title: "IRepD2ShapeObjBaseInt"
description: "The 2DShapeObject object provides the properties of the curve in a 2D axis system in DIAdem REPORT. The 2DShapeObject object corresponds to one of the following"
---

# IRepD2ShapeObjBaseInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DShapeObject

The 2DShapeObject object provides the properties of the curve in a 2D axis system in DIAdem REPORT. The 2DShapeObject object corresponds to one of the following objects: 2DBars (IRepD2ShapeObjBarsInt) Bars 2DBarsHorizontal (IRepD2ShapeObjBarsHorizontalInt) Horizontal bars 2DConstant (IRepD2ShapeObjConstantInt) Constant 2DCoordinate (IRepD2ShapeObjCoordinateInt) Coordinate 2DDifferential (IRepD2ShapeObjDifferentialInt) Differential 2DFilledArea (IRepD2ShapeObjFilledAreaInt) Filled area 2DGroupedBars (IRepD2ShapeObjBarsGroupedInt) Grouped bars 2DLine (IRepD2ShapeObjLineInt) Line 2DLineAndPoints (IRepD2ShapeObjLineAndPointsInt) Line and points 2DOutlineBars (IRepD2ShapeObjOutlineBarsInt) Outlined bars 2DOutlineBarsHorizontal (IRepD2ShapeObjOutlineBarsHorizontalInt) Horizontal outlined bars 2DSpecialCombination (IRepD2ShapeObjSpecialCombinationInt) Special combination 2DSpikes (IRepD2ShapeObjSpikesInt) Spikes 2DSpikesHorizontal (IRepD2ShapeObjSpikesHorizontalInt) Horizontal spikes 2DStackedBars (IRepD2ShapeObjBarsStackedInt) Stacked bars

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curveint/">2DCurve</a>.<a href="../../properties/irepd2curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBaseInt.htm`*
