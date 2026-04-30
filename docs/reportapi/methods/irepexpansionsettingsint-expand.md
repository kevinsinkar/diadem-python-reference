---
title: "IRepExpansionSettingsInt.Expand"
description: "Expands the curves in a REPORT layout. To create a layout with curve expansion, you must assign the value True to the property Enable for CurveExpansionSettings"
---

# IRepExpansionSettingsInt.Expand

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Expand for CurveExpansionSettings

Expands the curves in a REPORT layout. To create a layout with curve expansion, you must assign the value True to the property Enable for CurveExpansionSettings .

## Signature

```python
obj.Expand()
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
dd.Report.NewLayout()
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
oMyShape = oMyCurve.Shape
oMyShape.Settings.UseCurveExpansion = True
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"

dd.Report.Settings.CurveExpansion.Expand()
print ("Number of expanded curves: " , oMy2DAxisSystem.Curves2D.Count)
for oMyExpandedCurve in oMy2DAxisSystem.Curves2D:
    oMyExpandedCurve.Shape.Extensions.Marker.Type = dd.eMarkerCircle
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Expand_IRepExpansionSettingsInt.htm`*
