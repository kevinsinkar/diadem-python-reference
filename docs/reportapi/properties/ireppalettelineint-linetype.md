---
title: "IRepPaletteLineInt.LineType"
description: "Specifies the line style of the color palette in a 2D axis system in DIAdem REPORT."
---

# IRepPaletteLineInt.LineType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineType for PaletteLine

Specifies the line style of the color palette in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.LineType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineTypeNone` | 0 | None |
| `eLineTypeSolid` | 1 | Line |
| `eLineTypeDashDot` | 2 | Dots and dashes |
| `eLineTypeDashed1` | 3 | Dashes 1 |
| `eLineTypeDashed2` | 4 | Dashes 2 |
| `eLineTypeDotted` | 5 | Dotted |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
iChannelMax = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("minimum").Value
oMyLine = oMyCurve.Shape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyCurve.Shape.Settings.Palette.Lines
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

*Source: `ReportApi/properties/Report_property_LineType_IRepPaletteLineInt.htm`*
