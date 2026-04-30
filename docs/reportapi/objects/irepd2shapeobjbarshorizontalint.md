---
title: "IRepD2ShapeObjBarsHorizontalInt"
description: "The 2DBarsHorizontal object provides the curve properties of a 2D axis system in the Horizontal bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsHorizontalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBarsHorizontal

The 2DBarsHorizontal object provides the curve properties of a 2D axis system in the Horizontal bars display mode in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBarsHorizontal, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjbarshorizontalint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjbarshorizontalint-xchannel/">XChannel</a> | <a href="../../properties/irepd2shapeobjbarshorizontalint-ychannel/">YChannel</a></p>
</div>
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

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBarsHorizontalInt.htm`*
