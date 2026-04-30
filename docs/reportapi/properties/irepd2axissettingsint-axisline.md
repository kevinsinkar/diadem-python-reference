---
title: "IRepD2AxisSettingsInt.AxisLine"
description: "Specifies the properties of the axis lines in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisSettingsInt.AxisLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisLine for 2DAxisSettings

Specifies the properties of the axis lines in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.AxisLine
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMy2DAxisSystem.Settings.AxisLine.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
oMy2DAxisSystem.Settings.AxisLine.Width = dd.eLineWidth0100
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AxisLine_IRepD2AxisSettingsInt.htm`*
