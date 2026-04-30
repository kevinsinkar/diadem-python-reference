---
title: "IRepAttributeListInt.UseLineColor"
description: "Specifies whether DIAdem REPORT displays expanding curves in the colors specified in the attribute list."
---

# IRepAttributeListInt.UseLineColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseLineColor for AttributeList

Specifies whether DIAdem REPORT displays expanding curves in the colors specified in the attribute list.

## Signature

```python
obj.UseLineColor
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
oMyReportSettings = dd.Report.Settings
oMyCurveExpansion = oMyReportSettings.CurveExpansion
oMyCurveExpansion.Enable = True
oMyCurveExpansion.AttributeList.Enable = True
oMyCurveExpansion.AttributeList.UseLineColor = False
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.Settings.UseCurveExpansion = True
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseLineColor_IRepAttributeListInt.htm`*
