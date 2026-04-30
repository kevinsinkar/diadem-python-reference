---
title: "IRepD2AxisYInt.Line"
description: "Specifies the line properties of the y-axis in a 2D axis system in DIAdem REPORT. Assign the value TRUE to the property UseIndividualAxisStyle in order to assig"
---

# IRepD2AxisYInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 2DAxisY

Specifies the line properties of the y-axis in a 2D axis system in DIAdem REPORT. Assign the value TRUE to the property UseIndividualAxisStyle in order to assign different properties to the axes of a 2D axis system.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMy2DAxisSystem.YAxis.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD2AxisYInt.htm`*
