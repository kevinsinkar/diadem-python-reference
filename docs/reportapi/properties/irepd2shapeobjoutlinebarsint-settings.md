---
title: "IRepD2ShapeObjOutlineBarsInt.Settings"
description: "Specifies the curve properties in the Outlined bars display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjOutlineBarsInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DOutlineBars

Specifies the curve properties in the Outlined bars display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySettings = oMyShape.Settings
oMySettings.Line.Width = dd.eLineWidth0140
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepD2ShapeObjOutlineBarsInt.htm`*
