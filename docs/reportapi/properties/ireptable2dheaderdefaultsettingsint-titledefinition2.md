---
title: "IRepTable2DHeaderDefaultSettingsInt.TitleDefinition2"
description: "Specifies a predefined text in the global headers and footers of a 2D table in DIAdem REPORT."
---

# IRepTable2DHeaderDefaultSettingsInt.TitleDefinition2

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TitleDefinition2 for 2DTableColumnHeaderFooterDefaultSettings

Specifies a predefined text in the global headers and footers of a 2D table in DIAdem REPORT.

## Signature

```python
obj.TitleDefinition2
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
oMyHeaderSettings = oMy2DTable.Settings.Header
oMyHeaderSettings.TitleDefinition1 = dd.e2DTableTitleChnSumVisible
oMyHeaderSettings.TitleDefinition2 = dd.e2DTableTitleChnMinVisible
oMyHeaderSettings.TitleDefinition3 = dd.e2DTableTitleChnMaxVisible
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TitleDefinition2_IRepTable2DHeaderDefaultSettingsInt.htm`*
