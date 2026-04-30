---
title: "IRepTable2DColumnSettingsInt.Footer"
description: "Specifies the properties the footer of a column in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnSettingsInt.Footer

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Footer for 2DTableColumnSettings

Specifies the properties the footer of a column in a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.Footer
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
oMyCol2FooterIndividualSettings = oMyColumn2.Settings.Footer.IndividualSettings
oMyCol2FooterIndividualSettings.Enable = True
oMyCol2FooterIndividualSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyCol2FooterIndividualSettings = oMyColumn2.Settings.Footer.IndividualTitle
oMyCol2FooterIndividualSettings.Enable = True
oMyCol2FooterIndividualSettings.Title1 = "Footer 1"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Footer_IRepTable2DColumnSettingsInt.htm`*
