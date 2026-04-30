---
title: "IRepTable2DColumnFooterSettingsInt.IndividualSettings"
description: "Specifies the individual properties of the footers of a selected 2D table column in DIAdem REPORT. Assign the value True to the Enable property so that DIAdem d"
---

# IRepTable2DColumnFooterSettingsInt.IndividualSettings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndividualSettings for 2DTableColumnFooterSettings

Specifies the individual properties of the footers of a selected 2D table column in DIAdem REPORT. Assign the value True to the Enable property so that DIAdem displays the individual properties of the footers.

## Signature

```python
return_value = obj.IndividualSettings
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
oMyCol2FooterIndividualSettings= oMyColumn2.Settings.Footer.IndividualSettings
oMyCol2FooterIndividualSettings.Enable = True
oMyCol2FooterIndividualSettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndividualSettings_IRepTable2DColumnFooterSettingsInt.htm`*
