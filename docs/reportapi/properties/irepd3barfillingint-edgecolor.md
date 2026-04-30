---
title: "IRepD3BarFillingInt.EdgeColor"
description: "Specifies the line width of a bar display in a 3D axis system in DIAdem REPORT. DIAdem only includes the property EdgeColor if you assign the value TRUE to the "
---

# IRepD3BarFillingInt.EdgeColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Pattern for 3DBarFilling

Specifies the line width of a bar display in a 3D axis system in DIAdem REPORT. DIAdem only includes the property EdgeColor if you assign the value TRUE to the Enable property.

## Signature

```python
return_value = obj.EdgeColor
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.ePredefinedColorBlue)
oMyFilling = oMySettings.Filling
oMyFilling.Enable = True
oMyFilling.EdgeColor.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_EdgeColor_IRepD3BarFillingInt.htm`*
