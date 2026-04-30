---
title: "IRepTable2DColumnFooterSettingsInt.IndividualTitle"
description: "Specifies the individual properties of a footer in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnFooterSettingsInt.IndividualTitle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndividualTitle for 2DTableColumnFooterSettings

Specifies the individual properties of a footer in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.IndividualTitle
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
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
Col2FooterTitleSettings = oMyColumn2.Settings.Footer.IndividualTitle
Col2FooterTitleSettings.Enable = True
Col2FooterTitleSettings.Title1 = "Footer Text"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndividualTitle_IRepTable2DColumnFooterSettingsInt.htm`*
