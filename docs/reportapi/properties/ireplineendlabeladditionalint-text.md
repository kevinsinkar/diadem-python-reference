---
title: "IRepLineEndLabelAdditionalInt.Text"
description: "Specifies in a 2D axis system in DIAdem REPORT the text for the curve end. The text may also contain @@ expressions, such as @@MyFunc(Par)@@ , but not more than"
---

# IRepLineEndLabelAdditionalInt.Text

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Text for AdditionalLineEndLabel

Specifies in a 2D axis system in DIAdem REPORT the text for the curve end. The text may also contain @@ expressions, such as @@MyFunc(Par)@@ , but not more than one @@ expression.

## Signature

```python
obj.Text
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
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyEndLabel = oMyCurve.Shape.Extensions.EndLabel
oMyEndLabel.Position = dd.e2DLineEndLabelPositionLargestXValue
oMyEndLabel.Type = dd.e2DLineEndLabelCustomText
oMyEndLabel.Text = "End label"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Text_IRepLineEndLabelAdditionalInt.htm`*
