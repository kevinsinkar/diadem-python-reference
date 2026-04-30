---
title: "IRepD2ShapeObjSpecialCombinationInt"
description: "The 2DSpecialCombination object provides the curve properties of a 2D axis system in the Special combination display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSpecialCombination

The 2DSpecialCombination object provides the curve properties of a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyExtension = oMyCurve.Shape.Extensions
oMyExtension.Label.YValueVisible = True
oMyExtension.Label.YValueFormat = "d.dd"
oMyExtension.Label.Position.Type = dd.e2DLabelPositionAtPoint
oMyExtension.Label.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyExtension.Label.Repetition.NValue = 10
oMyExtension.AdditionalStyles.Type = dd.e2DAdditionalStyleSpikes
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjspecialcombinationint-extensions/">Extensions</a> | <a href="../../properties/irepd2shapeobjspecialcombinationint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjspecialcombinationint-xchannel/">XChannel</a> | <a href="../../properties/irepd2shapeobjspecialcombinationint-ychannel/">YChannel</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjSpecialCombinationInt.htm`*
