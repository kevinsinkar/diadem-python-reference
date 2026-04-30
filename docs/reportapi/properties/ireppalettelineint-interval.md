---
title: "IRepPaletteLineInt.Interval"
description: "Specifies the line interval for broken lines of the color palette in a 2D axis system in DIAdem REPORT. Greater values mean greater intervals."
---

# IRepPaletteLineInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for PaletteLine

Specifies the line interval for broken lines of the color palette in a 2D axis system in DIAdem REPORT. Greater values mean greater intervals.

## Signature

```python
obj.Interval
```

## Python example

```python
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMyReportObj.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyReportObj.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
iChannelMax = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("minimum").Value
oMyLine = oMyShape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyShape.Settings.Palette.Lines
i = 0
for oMyPaletteLine in oMyPalette:
    i = i + 1
    oMyPaletteLine.LineType = dd.eLineTypeDashDot
    oMyPaletteLine.Interval = 10
    oMyPaletteLine.Width = dd.eLineWidth0035
    oMyPaletteLine.UpperLimit = iChannelMin + (iChannelMax - iChannelMin) / oMyPalette.Count * i
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepPaletteLineInt.htm`*
