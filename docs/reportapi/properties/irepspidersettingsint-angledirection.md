---
title: "IRepSpiderSettingsInt.AngleDirection"
description: "Specifies the angle direction of the label of a spider axis system in DIAdem REPORT."
---

# IRepSpiderSettingsInt.AngleDirection

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AngleDirection for SpiderSettings

Specifies the angle direction of the label of a spider axis system in DIAdem REPORT.

## Signature

```python
obj.AngleDirection
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngleDirectionCounterClockwise` | 0 | Counter clockwise |
| `eAngleDirectionClockwise` | 1 | Clockwise |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyAxisSystemSettings = oMyAxisSystem.Settings
oMyAxisSystemSettings.DisplayMode = dd.eSpiderDisplayModeSpider
oMyAxisSystemSettings.ShowBorder = True
oMyAxisSystemSettings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed
oMyAxisSystemSettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
oMyAxisSystemSettings.AngleDirection = dd.eAngleDirectionClockwise

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AngleDirection_IRepSpiderSettingsInt.htm`*
