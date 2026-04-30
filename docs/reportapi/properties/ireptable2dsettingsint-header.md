---
title: "IRepTable2DSettingsInt.Header"
description: "Specifies the properties of the headers and footers of a 2D table in DIAdem REPORT."
---

# IRepTable2DSettingsInt.Header

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Header for 2DTableSettings

Specifies the properties of the headers and footers of a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Header
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
oMySettings = oMy2DTable.Settings
oMySettings.Header.Height = 20
oMySettings.BackgroundColor.SetPredefinedColor(dd.eColorIndexGrey )
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

*Source: `ReportApi/properties/Report_property_Header_IRepTable2DSettingsInt.htm`*
