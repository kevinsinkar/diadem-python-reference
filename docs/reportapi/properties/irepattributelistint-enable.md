---
title: "IRepAttributeListInt.Enable"
description: "Specifies whether DIAdem REPORT uses the attribute list for the curve expansion in an axis system."
---

# IRepAttributeListInt.Enable

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Enable for AttributeList

Specifies whether DIAdem REPORT uses the attribute list for the curve expansion in an axis system.

## Signature

```python
obj.Enable
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
oMyReportSettings = dd.Report.Settings
oMyReportSettings.CurveExpansion.Enable = True
oMyReportSettings.CurveExpansion.AttributeList.Enable = True

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.Settings.UseCurveExpansion = True
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
oMyCurveLegend = oMy2DaxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyCurveLegend.Settings.ShowOnlyFirstCurve = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Enable_IRepAttributeListInt.htm`*
