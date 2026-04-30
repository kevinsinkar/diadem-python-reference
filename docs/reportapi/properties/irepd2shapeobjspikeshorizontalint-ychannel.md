---
title: "IRepD2ShapeObjSpikesHorizontalInt.YChannel"
description: "Specifies the y-channel of a curve in the Horizontal spikes display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjSpikesHorizontalInt.YChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannel for 2DSpikesHorizontal

Specifies the y-channel of a curve in the Horizontal spikes display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.YChannel
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\Report_EXPL","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpikesHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMyShape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyShape.Settings.Line.Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannel_IRepD2ShapeObjSpikesHorizontalInt.htm`*
