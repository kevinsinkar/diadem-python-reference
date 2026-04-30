---
title: "IRepTable2DHeaderDefaultSettingsInt.UseAutoFontSize"
description: "Specifies whether DIAdem REPORT determines the font size of the headers and footers of a 2D table automatically."
---

# IRepTable2DHeaderDefaultSettingsInt.UseAutoFontSize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseAutoFontSize for 2DTableHeaderFooterDefaultSettings

Specifies whether DIAdem REPORT determines the font size of the headers and footers of a 2D table automatically.

## Signature

```python
obj.UseAutoFontSize
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
oMyHeaderSettings.UseAutoFontSize = False
oMyHeaderSettings.Font.Size = 4
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

*Source: `ReportApi/properties/Report_property_UseAutoFontSize_IRepTable2DHeaderDefaultSettingsInt.htm`*
