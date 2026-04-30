---
title: "IRepD2ShapeObjLineAndPointsExtensionsInt.Label"
description: "Specifies the curve labels in the Line and points display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjLineAndPointsExtensionsInt.Label

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Label for 2DLineAndPointsExtensions

Specifies the curve labels in the Line and points display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Label
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyLabel = oMyShape.Extensions.Label
oMyLabel.TextVisible = True
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 20
oMyLabel.Text = "*"
oMyLabel.Font.Size = 7
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Label_IRepD2ShapeObjLineAndPointsExtensionsInt.htm`*
