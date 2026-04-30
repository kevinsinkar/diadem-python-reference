---
title: "IRepD2ShapeObjSpecialCombinationExtensionsInt.EndLabel"
description: "Specifies the properties of the curve end label in a 2D axis system in the Special combination display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationExtensionsInt.EndLabel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: EndLabel for 2DSpecialCombinationExtensions

Specifies the properties of the curve end label in a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.EndLabel
```

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
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMySetting.ConnectNoValueNeighbors = True
oMyEndLabel = oMyShape.Extensions.EndLabel
oMyEndLabel.Position = dd.e2DLineEndLabelPositionLargestXValue
oMyEndLabel.Type = dd.e2DLineEndLabelCustomText
oMyEndLabel.Text = "End Label"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_EndLabel_IRepD2ShapeObjSpecialCombinationExtensionsInt.htm`*
