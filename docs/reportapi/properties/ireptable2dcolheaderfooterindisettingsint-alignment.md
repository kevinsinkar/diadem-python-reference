---
title: "IRepTable2DColHeaderFooterIndiSettingsInt.Alignment"
description: "Specifies the relative position of the column headers and footers of a selected 2D table column in DIAdem REPORT."
---

# IRepTable2DColHeaderFooterIndiSettingsInt.Alignment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Alignment for 2DTableColumnHeaderFooterIndividualSettings

Specifies the relative position of the column headers and footers of a selected 2D table column in DIAdem REPORT.

## Signature

```python
obj.Alignment
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTableAlignmentDecimalPoint` | 3 |  |

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
Col2HeadSettings = oMyColumn2.Settings.Header.IndividualSettings
Col2HeadSettings.Enable = True
Col2HeadSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
Col2HeadSettings.Alignment = dd.e2DTableAlignmentRight
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Alignment_IRepTable2DColHeaderFooterIndiSettingsInt.htm`*
