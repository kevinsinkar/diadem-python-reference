---
title: "IRepTable2DSettingsInt.ColumnExpansionMode"
description: "Specifies the sorting of the columns in a 2D table in DIAdem REPORT. To use the ColumnExpansionMode property, you must first enable the expansion mode with the "
---

# IRepTable2DSettingsInt.ColumnExpansionMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColumnExpansionMode for 2DTableSettings

Specifies the sorting of the columns in a 2D table in DIAdem REPORT. To use the ColumnExpansionMode property, you must first enable the expansion mode with the Enable for CurveExpansionSettings property.

## Signature

```python
obj.ColumnExpansionMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColumnExpansionModeUseDefault` | 0 | Sorts the columns of the table as specified in the general settings in DIAdem REPORT under Settings » Layout Setup » Layout Parameters »Display»Sort . |
| `eColumnExpansionModeSortByGroups` | 1 | Sorts the columns of the table so that the first columns receive the first channel for display of the first expanded group. The next columns contain the first channel of the second expanded group, and so on. This is followed by the second channel of the first expanded group, then the second channel of the second expanded group, and so on. |
| `eColumnExpansionModeSortByChannels` | 2 | Sorts the table columns so that the first columns receive all the channels to be displayed of the first expanded group. The next columns contain all channels  to be displayed of the second expanded group, and so on. |

## Python example

```python
dd.Data.Root.Clear()
dd.Report.NewLayout()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
oMyReportSettings = dd.Report.Settings
oMyReportSettings.CurveExpansion.Enable = True
oMyReportSettings.CurveExpansion.AttributeList.Enable = True
oMyReportSettings.CurveExpansion.Mode = dd.eCurveExpansionModeSortByChannels
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyTableSettings = oMy2DTable.Settings
oMyTableSettings.ColumnExpansionMode = dd.eColumnExpansionModeUseDefault
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "*/Temp_A"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "*/Temp_B"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColumnExpansionMode_IRepTable2DSettingsInt.htm`*
