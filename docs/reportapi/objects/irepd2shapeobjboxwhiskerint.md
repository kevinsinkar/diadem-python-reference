---
title: "IRepD2ShapeObjBoxWhiskerInt"
description: "The 2DBoxWhisker object provides the properties of a curve of a 2D axis system in the Box Whisker display mode."
---

# IRepD2ShapeObjBoxWhiskerInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBoxWhisker

The 2DBoxWhisker object provides the properties of a curve of a 2D axis system in the Box Whisker display mode.

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
<p><a href="../../properties/irepd2shapeobjboxwhiskerint-extensions/">Extensions</a> | <a href="../../properties/irepd2shapeobjboxwhiskerint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjboxwhiskerint-xchannel/">XChannel</a> | <a href="../../properties/irepd2shapeobjboxwhiskerint-ychannels/">YChannels</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curveint/">2DCurve</a>.<a href="../../properties/irepd2curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBoxWhiskerInt.htm`*
