---
title: "IRepTable2DColHeaderFooterIndiTitlesSettingsInt.Title3"
description: "Specifies headers and footers of a selected 2D table column in DIAdem REPORT."
---

# IRepTable2DColHeaderFooterIndiTitlesSettingsInt.Title3

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Title3 for 2DTableColumnHeaderFooterIndividualTitleSettings

Specifies headers and footers of a selected 2D table column in DIAdem REPORT.

## Signature

```python
obj.Title3
```

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMy2DTable.Settings.Header.Height = 20
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
Col2HeadSettings = oMyColumn2.Settings.Header.IndividualSettings
Col2HeadSettings.Enable = True
Col2HeadSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
Col2TitleSettings = oMyColumn2.Settings.Header.IndividualTitle
Col2TitleSettings.Enable = True
Col2TitleSettings.Title1 = "Title 1"
Col2TitleSettings.Title2 = "Title 2"
Col2TitleSettings.Title3 = "Title 3"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Title3_IRepTable2DColHeaderFooterIndiTitlesSettingsInt.htm`*
