---
title: "IRepSpiderSettingsInt.BackgroundColor"
description: "Specifies the background color of a spider axis system in DIAdem REPORT."
---

# IRepSpiderSettingsInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for SpiderSettings

Specifies the background color of a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMySpiderSettings = oMyAxisSystem.Settings
oMySpiderSettings.DisplayMode = dd.eSpiderDisplayModeSpider
oMySpiderSettings.ShowBorder = True
oMySpiderSettings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed
oMySpiderSettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
oMySpiderSettings.AngleDirection = dd.eAngleDirectionClockwise

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepSpiderSettingsInt.htm`*
