---
title: "IRepD2SpecialCombAdditionalStylesInt.Width"
description: "Specifies the width of a bar in the special type Bars in the Special combination display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2SpecialCombAdditionalStylesInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for 2DAdditionalStyles

Specifies the width of a bar in the special type Bars in the Special combination display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Width
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
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyAdditionalStyles = oMyShape.Extensions.AdditionalStyles
oMyAdditionalStyles.Type = dd.e2DAdditionalStyleBars
oMyAdditionalStyles.Line.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyAdditionalStyles.Width = 50
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepD2SpecialCombAdditionalStylesInt.htm`*
