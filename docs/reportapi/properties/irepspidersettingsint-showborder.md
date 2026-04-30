---
title: "IRepSpiderSettingsInt.ShowBorder"
description: "Specifies whether DIAdem REPORT frames a spider axis system."
---

# IRepSpiderSettingsInt.ShowBorder

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowBorder for SpiderSettings

Specifies whether DIAdem REPORT frames a spider axis system.

## Signature

```python
obj.ShowBorder
```

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

oMyAxisSystemSettings = oMyAxisSystem.Settings
oMyAxisSystemSettings.DisplayMode = dd.eSpiderDisplayModeSpider
oMyAxisSystemSettings.ShowBorder = True
oMyAxisSystemSettings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed
oMyAxisSystemSettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
oMyAxisSystemSettings.AngleDirection = dd.eAngleDirectionClockwise

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowBorder_IRepSpiderSettingsInt.htm`*
