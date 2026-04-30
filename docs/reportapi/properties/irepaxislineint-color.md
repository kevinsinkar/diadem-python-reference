---
title: "IRepAxisLineInt.Color"
description: "Specifies the line color of an axis in a 2D axis system in DIAdem REPORT. DIAdem only includes the property Color if you assign the value FALSE to the UseCurveC"
---

# IRepAxisLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for AxisLine

Specifies the line color of an axis in a 2D axis system in DIAdem REPORT. DIAdem only includes the property Color if you assign the value FALSE to the UseCurveColor property.

## Signature

```python
return_value = obj.Color
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
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXLine = oMy2DAxisSystem.XAxis.Line
oMyXLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyXLine.UseCurveColor = False
oMyXLine.Width = dd.eLineWidth0100
oMyYLine = oMy2DAxisSystem.YAxis.Line
oMyYLine.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyYLine.UseCurveColor = False
oMyYLine.Width = dd.eLineWidth0100
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepAxisLineInt.htm`*
