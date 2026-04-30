---
title: "IRepPaletteLineInt.Width"
description: "Specifies the line width of a legend in DIAdem REPORT."
---

# IRepPaletteLineInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for PaletteLine

Specifies the line width of a legend in DIAdem REPORT.

## Signature

```python
obj.Width
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineWidthMin` | 0 | Minimum |
| `eLineWidth0025` | 1 | 0.25 |
| `eLineWidth0035` | 2 | 0.35 |
| `eLineWidth0050` | 3 | 0.5 |
| `eLineWidth0070` | 4 | 0.7 |
| `eLineWidth0100` | 5 | 1.0 |
| `eLineWidth0140` | 6 | 1.4 |
| `eLineWidth0200` | 7 | 2.0 |
| `eLineWidth0280` | 8 | 2.8 |
| `eLineWidth0400` | 9 | 4.0 |
| `eLineWidth0560` | 10 | 5.6 |
| `eLineWidth0800` | 11 | 8.0 |
| `eLineWidth1120` | 12 | 11.2 |
| `eLineWidth1600` | 13 | 16.0 |
| `eLineWidth2240` | 14 | 22.4 |
| `eLineWidth3200` | 15 | 32.0 |

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

*Source: `ReportApi/properties/Report_property_Width_IRepPaletteLineInt.htm`*
