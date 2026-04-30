---
title: "IRepExpansionSettingsInt.Collapse"
description: "Deletes the expanded curves of a REPORT layout to make changes to the expanded curves. DIAdem expands the curves of a layout with curve expansion when you call "
---

# IRepExpansionSettingsInt.Collapse

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Collapse for CurveExpansionSettings

Deletes the expanded curves of a REPORT layout to make changes to the expanded curves. DIAdem expands the curves of a layout with curve expansion when you call the Refresh method or the Expand method. To create a layout with curve expansion, you must assign the value True to the property Enable for CurveExpansionSettings .

## Signature

```python
obj.Collapse()
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
dd.Report.Refresh()
print ("Before collapse, number of expanded curves: " , oMy2DAxisSystem.Curves2D.Count)
dd.Report.Settings.CurveExpansion.Collapse()
print ("After collapse, number of expanded curves: " , oMy2DAxisSystem.Curves2D.Count)
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

*Source: `ReportApi/methods/Report_method_Collapse_IRepExpansionSettingsInt.htm`*
