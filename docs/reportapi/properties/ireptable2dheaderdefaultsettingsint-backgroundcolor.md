---
title: "IRepTable2DHeaderDefaultSettingsInt.BackgroundColor"
description: "Specifies the background color of the headers and footers in a 2D table in DIAdem REPORT."
---

# IRepTable2DHeaderDefaultSettingsInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for 2DTableHeaderFooterDefaultSettings

Specifies the background color of the headers and footers in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
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
oMyHeaderSettings = oMy2DTable.Settings.Header
oMyHeaderSettings.Height = 20
oMyHeaderSettings.Title1 = "@@ChnName(CurrChnNo)@@"
oMyHeaderSettings.Title2 = "@@ChnDim(CurrChnNo)@@"
oMyHeaderSettings.Font.Size = 4
oMyHeaderSettings.BackgroundColor.ColorIndex = dd.eColorIndexGreen
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepTable2DHeaderDefaultSettingsInt.htm`*
