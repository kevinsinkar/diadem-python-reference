---
title: "IRepD2ShapeObjBarsExtensionsInt"
description: "The 2DBarsExtensions object provides the extended properties of a curve in the Bars display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjBarsExtensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBarsExtensions

The 2DBarsExtensions object provides the extended properties of a curve in the Bars display mode in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm")
dd.Report.NewLayout()

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"

oMyExtensions = oMyShape.Extensions
oMyExtensions.Label.TextVisible = True
oMyExtensions.Label.RelativePosition = dd.eRelativePositionPointTop
oMyExtensions.Label.YValueVisible = True
oMyExtensions.Label.YValueFormat = "d.d"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjbarsextensionsint-label/">Label</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjbarsint/">2DBars</a>.<a href="../../properties/irepd2shapeobjbarsint-extensions/">Extensions</a> | <a href="../irepd2shapeobjbarsgroupedint/">2DGroupedBars</a>.<a href="../../properties/irepd2shapeobjbarsgroupedint-extensions/">Extensions</a> | <a href="../irepd2shapeobjbarsstackedint/">2DStackedBars</a>.<a href="../../properties/irepd2shapeobjbarsstackedint-extensions/">Extensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBarsExtensionsInt.htm`*
