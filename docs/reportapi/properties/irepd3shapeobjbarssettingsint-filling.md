---
title: "IRepD3ShapeObjBarsSettingsInt.Filling"
description: "Specifies the filling properties of a curve in the Bars display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjBarsSettingsInt.Filling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Filling for 3DBarsSettings

Specifies the filling properties of a curve in the Bars display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Filling
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
oMySettings.Line.Color.SetPredefinedColor(dd.ePredefinedColorGreen)
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

*Source: `ReportApi/properties/Report_property_Filling_IRepD3ShapeObjBarsSettingsInt.htm`*
