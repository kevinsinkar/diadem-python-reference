---
title: "IRepD2AxisXInt.Line"
description: "Specifies the line properties of the x-axis in a 2D axis system in DIAdem REPORT. Assign the value TRUE to the property UseIndividualAxisStyle in order to assig"
---

# IRepD2AxisXInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 2DAxisX

Specifies the line properties of the x-axis in a 2D axis system in DIAdem REPORT. Assign the value TRUE to the property UseIndividualAxisStyle in order to assign different properties to the axes of a 2D axis system.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.Y1 = 20
oMyPos.X2 = 80
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMy2DAxisSystem.XAxis.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD2AxisXInt.htm`*
