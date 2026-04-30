---
title: "2DCurves"
description: "Collection of all 2DCurve objects in DIAdem REPORT. Use the 2DCurves collection to delete or to create new curves in 2D axis systems."
---

# 2DCurves

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DCurves

Collection of all 2DCurve objects in DIAdem REPORT. Use the 2DCurves collection to delete or to create new curves in 2D axis systems.

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2curvelistint-count/">Count</a> | <a href="../../properties/irepd2curvelistint-defaultshapetype/">DefaultShapeType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2curvelistint-add/">Add</a> | <a href="../../methods/irepd2curvelistint-changeshape/">ChangeShape</a> | <a href="../../methods/irepd2curvelistint-copy/">Copy</a> | <a href="../../methods/irepd2curvelistint-exists/">Exists</a> | <a href="../../methods/irepd2curvelistint-item/">Item</a> | <a href="../../methods/irepd2curvelistint-move/">Move</a> | <a href="../../methods/irepd2curvelistint-remove/">Remove</a> | <a href="../../methods/irepd2curvelistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-curves2d/">Curves2D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2CurveListInt.htm`*
