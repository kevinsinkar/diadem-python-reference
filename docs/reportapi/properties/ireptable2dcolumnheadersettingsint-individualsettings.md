---
title: "IRepTable2DColumnHeaderSettingsInt.IndividualSettings"
description: "Specifies the individual properties of the headers and footers of a selected 2D table column in DIAdem REPORT. Assign the value True to the Enable property so t"
---

# IRepTable2DColumnHeaderSettingsInt.IndividualSettings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndividualSettings for 2DTableColumnHeaderSettings

Specifies the individual properties of the headers and footers of a selected 2D table column in DIAdem REPORT. Assign the value True to the Enable property so that DIAdem displays the individual properties of the headers and footers.

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
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
Col2HeadIndividualSettings = oMyColumn2.Settings.Header.IndividualSettings
Col2HeadIndividualSettings.Enable = True
Col2HeadIndividualSettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndividualSettings_IRepTable2DColumnHeaderSettingsInt.htm`*
