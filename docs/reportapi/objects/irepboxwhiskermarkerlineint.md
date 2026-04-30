---
title: "IRepBoxWhiskerMarkerLineInt"
description: "The 2DBoxWhiskerMarkerLine object provides the line properties of an additional marker in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerMarkerLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBoxWhiskerMarkerLine

The 2DBoxWhiskerMarkerLine object provides the line properties of an additional marker in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

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
oMyShape.Extensions.MarkerWhisker.Type = dd.eMarkerCircle
oMyShape.Extensions.MarkerWhisker.Line.UseBorderColor = False
oMyShape.Extensions.MarkerWhisker.Line.Color.ColorIndex = dd.eColorIndexRed
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepboxwhiskermarkerlineint-color/">Color</a> | <a href="../../properties/irepboxwhiskermarkerlineint-usebordercolor/">UseBorderColor</a> | <a href="../../properties/irepboxwhiskermarkerlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepboxwhiskermarkerint/">2DBoxWhiskerMarker</a>.<a href="../../properties/irepboxwhiskermarkerint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepBoxWhiskerMarkerLineInt.htm`*
