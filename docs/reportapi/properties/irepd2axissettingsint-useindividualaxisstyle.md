---
title: "IRepD2AxisSettingsInt.UseIndividualAxisStyle"
description: "Specifies whether DIAdem REPORT displays the axes of a 2D axis system in different colors and line widths."
---

# IRepD2AxisSettingsInt.UseIndividualAxisStyle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseIndividualAxisStyle for 2DAxisSettings

Specifies whether DIAdem REPORT displays the axes of a 2D axis system in different colors and line widths.

## Signature

```python
obj.UseIndividualAxisStyle
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
oMy2DAxisSystem.XAxis.Line.Color.SetPredefinedColor(dd.eColorIndexViolet)
oMy2DAxisSystem.YAxis.Line.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseIndividualAxisStyle_IRepD2AxisSettingsInt.htm`*
