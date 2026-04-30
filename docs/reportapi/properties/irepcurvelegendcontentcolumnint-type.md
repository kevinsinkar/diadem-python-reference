---
title: "IRepCurvelegendContentColumnInt.Type"
description: "Specifies whether DIAdem labels the legend of an axis system with user defined text or with default text."
---

# IRepCurvelegendContentColumnInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for CurveLegendColumn

Specifies whether DIAdem labels the legend of an axis system with user defined text or with default text.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendTextChannelName` | 0 | Channel name—DIAdem labels the legend symbol with the name of the y-channel of the associated curve. |
| `eLegendTextChannelNameFileName` | 1 | Channel name (filename)—DIAdem labels the legend symbol with the channel name and with the name of the file from which DIAdem loaded the channel. |
| `eLegendTextChannelNameFilePath` | 2 | Channel name (file path)—DIAdem labels the legend symbol with the channel name, with the name of the file from which DIAdem loaded the channel, and with the file path . |
| `eLegendTextChannelNameOriginAbbreviated` | 3 | Channel name (origin abbr.)—DIAdem labels the legend symbol with the channel name and with short information on the origin of the file from which DIAdem loaded the channel. |
| `eLegendTextChannelNameOrigin` | 4 | Channel name (origin)—DIAdem labels the legend symbol with the channel name and with detailed information on the origin of the file from which DIAdem loaded the channel. |
| `eLegendTextComment` | 5 | Channel comment—DIAdem labels the legend symbol with the comment of the y-channel of the associated curve. |
| `eLegendTextCustomText` | 6 | Free text—DIAdem uses the label text you enter for all legend symbols, for example, @@CN(CCN)@@ [@@CD(CCN)@@] , so that the program displays the channel name and the unit. |
| `eLegendTextCurveRelatedText` | 7 | Curve-related text—DIAdem labels each legend symbol with the free text you enter. |
| `eLegendTextChannelGroup` | 8 | Channel group—DIAdem labels each legend symbol with the channel group. |
| `eLegendTextChannelNameUnit` | 9 | Channel name and unit—DIAdem labels the legend symbol with the name of and the unit of the y-channel of the associated curve. |
| `eLegendTextChannelGroupChannelName` | 10 | Group name/Channel name—DIAdem labels the legend symbol with the group name and the name of the y-channel from the associated curve. |
| `eLegendTextChannelGroupChannelNameUnit` | 11 | Group name/Channel name and unit—DIAdem labels the legend symbol with the group name, name, and unit of the y-channel of the associated curve. |

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 30
oMyPosition.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMyShape = oMy2DCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMy2DaxisSystem.CurveLegend.Visible = True
oMyCurveLegendPos = oMy2DaxisSystem.CurveLegend.Position
oMyCurveLegendPos.RelativePosition = dd.eLegendRelativePositionBottomRight
oMyCurveLegendPos.SizeMode = dd.eLegendSizeElementwise
oMyCurveLegendPos.ElementHeight = 6
oMyCurveLegendPos.ElementWidth = 35
oMy2DaxisSystem.CurveLegend.Settings.Font.Size = 4
oMyLegendColumns = oMy2DaxisSystem.CurveLegend.Columns
oMyLegendColumns.Add()
oMyLegendColumns(1).Title = "First title"
oMyLegendColumns(1).Type = dd.eLegendTextCustomText
oMyLegendColumns(1).RelativeWidth = 2
oMyLegendColumns(1).Text = "First col - longer text"
oMyLegendColumns(2).Title = "Second title"
oMyLegendColumns(2).Type = dd.eLegendTextCustomText
oMyLegendColumns(2).RelativeWidth = 1
oMyLegendColumns(2).Text = "Second col"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepCurvelegendContentColumnInt.htm`*
