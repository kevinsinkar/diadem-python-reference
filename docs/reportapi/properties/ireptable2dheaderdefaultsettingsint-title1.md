---
title: "IRepTable2DHeaderDefaultSettingsInt.Title1"
description: "Specifies the global headers and footers of a 2D table in DIAdem REPORT."
---

# IRepTable2DHeaderDefaultSettingsInt.Title1

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Title1 for 2DTableHeaderFooterDefaultSettings

Specifies the global headers and footers of a 2D table in DIAdem REPORT.

## Signature

```python
obj.Title1
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
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
oMyHeaderSettings = oMy2DTable.Settings.Header
oMyHeaderSettings.Height = 20
oMyHeaderSettings.Title1 = "@@ChnName(CurrChnNo)@@"
oMyHeaderSettings.Title2 = "@@ChnDim(CurrChnNo)@@"
oMyHeaderSettings.Font.Size = 4
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Title1_IRepTable2DHeaderDefaultSettingsInt.htm`*
