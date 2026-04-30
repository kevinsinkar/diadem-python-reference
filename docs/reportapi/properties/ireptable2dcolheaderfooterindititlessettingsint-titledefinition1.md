---
title: "IRepTable2DColHeaderFooterIndiTitlesSettingsInt.TitleDefinition1"
description: "Specifies a predefined text in the headers and footers of a selected 2D table column in DIAdem REPORT."
---

# IRepTable2DColHeaderFooterIndiTitlesSettingsInt.TitleDefinition1

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TitleDefinition1 for 2DTableColumnHeaderFooterIndividualTitleSettings

Specifies a predefined text in the headers and footers of a selected 2D table column in DIAdem REPORT.

## Signature

```python
obj.TitleDefinition1
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
oMy2DTable.Settings.Footer.Height = 20
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[2]"
Col1FooterSettings = oMyColumn1.Settings.Footer.IndividualSettings
Col1FooterSettings.Enable = True
Col1FooterSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
Col1TitleSettings = oMyColumn1.Settings.Footer.IndividualTitle
Col1TitleSettings.Enable = True
Col1TitleSettings.TitleDefinition1 = dd.e2DTableTitleChnSumVisible
Col1TitleSettings.TitleDefinition2 = dd.e2DTableTitleChnMinVisible
Col1TitleSettings.TitleDefinition3 = dd.e2DTableTitleChnMaxVisible
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TitleDefinition1_IRepTable2DColHeaderFooterIndiTitlesSettingsInt.htm`*
