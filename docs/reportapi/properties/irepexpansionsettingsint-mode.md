---
title: "IRepExpansionSettingsInt.Mode"
description: "Specifies in which order DIAdem REPORT expands channels in a 2D axis system. If you assign the value eCurveExpansionModeSortByGroups to the Mode property, DIAde"
---

# IRepExpansionSettingsInt.Mode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Mode for CurveExpansionSettings

Specifies in which order DIAdem REPORT expands channels in a 2D axis system. If you assign the value eCurveExpansionModeSortByGroups to the Mode property, DIAdem REPORT first plots all original curves and then the expanded curves. If you assign the value eCurveExpansionModeSortByChannels to the Mode variable, DIAdem first plots the first curve and the associated expanded curves and the other curves in the same order.

## Signature

```python
obj.Mode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCurveExpansionModeSortByGroups` | 0 | Sort by groups |
| `eCurveExpansionModeSortByChannels` | 1 | Sort by channels |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
dd.Report.NewLayout()
oMyReportSettings = dd.Report.Settings
oMyReportSettings.CurveExpansion.Enable = True
oMyReportSettings.CurveExpansion.AttributeList.Enable = True
oMyReportSettings.CurveExpansion.Mode = dd.eCurveExpansionModeSortByGroups

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve1 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBars, "MyCurve1")
oMyShape1 = oMyCurve1.Shape
oMyShape1.Settings.FillEffects.Color.SetPredefinedColor(dd.ePredefinedColorYellow)
oMyShape1.Settings.UseCurveExpansion = True
oMyShape1.XChannel.Reference = ""
oMyShape1.YChannel.Reference = "Temp_A"
oMyCurve2 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBars, "MyCurve2")
oMyShape2 = oMyCurve2.Shape
oMyShape2.Settings.FillEffects.Color.SetPredefinedColor(dd.ePredefinedColorRed)
oMyShape2.Settings.UseCurveExpansion = True
oMyShape2.XChannel.Reference = ""
oMyShape2.YChannel.Reference = "Temp_B"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Mode_IRepExpansionSettingsInt.htm`*
