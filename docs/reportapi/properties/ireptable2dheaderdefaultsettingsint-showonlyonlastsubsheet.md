---
title: "IRepTable2DHeaderDefaultSettingsInt.ShowOnlyOnLastSubSheet"
description: "Specifies that DIAdem REPORT only displays footers at the end of the table. DIAdem only includes this property if you did not assign the value e2DTableIndexMode"
---

# IRepTable2DHeaderDefaultSettingsInt.ShowOnlyOnLastSubSheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowOnlyOnLastSubSheet for 2DTableColumnHeaderFooterDefaultSettings

Specifies that DIAdem REPORT only displays footers at the end of the table. DIAdem only includes this property if you did not assign the value e2DTableIndexModeAutomaticallyIncreasing to the IndexMode for 2DTableSettings property.

## Signature

```python
obj.ShowOnlyOnLastSubSheet
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
oMyFooterSettings = oMy2DTable.Settings.Footer
oMyFooterSettings.Height = 20
oMyFooterSettings.TitleDefinition1 = dd.e2DTableTitleChnSumAll
oMyFooterSettings.ShowOnlyOnLastSubSheet = True
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticallyIncreasing
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowOnlyOnLastSubSheet_IRepTable2DHeaderDefaultSettingsInt.htm`*
