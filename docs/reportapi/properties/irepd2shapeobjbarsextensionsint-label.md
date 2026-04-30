---
title: "IRepD2ShapeObjBarsExtensionsInt.Label"
description: "Specifies the curve labels in the Bars display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjBarsExtensionsInt.Label

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Label for 2DBarsExtensions

Specifies the curve labels in the Bars display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Label
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[2]"

oMyExtensions = oMyShape.Extensions
oMyExtensions.Label.TextVisible = True
oMyExtensions.Label.RelativePosition = dd.eRelativePositionPointTop
oMyExtensions.Label.YValueVisible = True
oMyExtensions.Label.YValueFormat = "d.d"

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Label_IRepD2ShapeObjBarsExtensionsInt.htm`*
