---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt"
description: "The 2DBoxWhiskerSettings object provides the properties of the curve parameters of a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBoxWhiskerSettings

The 2DBoxWhiskerSettings object provides the properties of the curve parameters of a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\EXPL_Legend.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBoxWhisker, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyYChannels= oMyShape.YChannels
oMyYChannels.RemoveAll()
oMyYChannels.Add("[1]/X_Channel")
oMyYChannels.Add("[1]/Z_Channel_1")
oMyYChannels.Add("[1]/Z_Channel_2")
oMyYChannels.Add("[1]/Z_Channel_3")
oMyYChannels.Add("[1]/Z_Channel_4")
oMyYChannels.Add("[1]/Z_Channel_5")

oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjboxwhiskersettingsint-borderline/">BorderLine</a> | <a href="../../properties/irepd2shapeobjboxwhiskersettingsint-filling/">Filling</a> | <a href="../../properties/irepd2shapeobjboxwhiskersettingsint-medianline/">MedianLine</a> | <a href="../../properties/irepd2shapeobjboxwhiskersettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjboxwhiskersettingsint-whiskerline/">WhiskerLine</a> | <a href="../../properties/irepd2shapeobjboxwhiskersettingsint-whiskermode/">WhiskerMode</a> | <a href="../../properties/irepd2shapeobjboxwhiskersettingsint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjboxwhiskerint/">2DBoxWhisker</a>.<a href="../../properties/irepd2shapeobjboxwhiskerint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*
