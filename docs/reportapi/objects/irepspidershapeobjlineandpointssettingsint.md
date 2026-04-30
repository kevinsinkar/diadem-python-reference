---
title: "IRepSpiderShapeObjLineAndPointsSettingsInt"
description: "The SpiderLineAndPointsSettings object provides the properties of a curve in the Line and points display mode in a spider axis system in DIAdem REPORT."
---

# IRepSpiderShapeObjLineAndPointsSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderLineAndPointsSettings

The SpiderLineAndPointsSettings object provides the properties of a curve in the Line and points display mode in a spider axis system in DIAdem REPORT.

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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMySpiderLineSettings = oMyCurve.Shape.Settings
oMySpiderLineSettings.Line.LineType = dd.eLineTypeDashed2
oMySpiderLineSettings.Type = dd.eSpiderLineStaired

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspidershapeobjlineandpointssettingsint-filleffects/">FillEffects</a> | <a href="../../properties/irepspidershapeobjlineandpointssettingsint-line/">Line</a> | <a href="../../properties/irepspidershapeobjlineandpointssettingsint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidershapeobjlineandpointsint/">SpiderLineAndPoints</a>.<a href="../../properties/irepspidershapeobjlineandpointsint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderShapeObjLineAndPointsSettingsInt.htm`*
