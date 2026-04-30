---
title: "IRepTable2DIndexSettingsInt.IndexEnd"
description: "Specifies the last row of the data channel, the values of which DIAdem REPORT displays in the 2D table. DIAdem only includes the IndexEnd property if you assign"
---

# IRepTable2DIndexSettingsInt.IndexEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndexEnd for 2DTableIndexSettings

Specifies the last row of the data channel, the values of which DIAdem REPORT displays in the 2D table. DIAdem only includes the IndexEnd property if you assign the value e2DTableIndexModeFixed to the IndexMode property.

## Signature

```python
obj.IndexEnd
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
oMyIndexSettings = oMy2DTable.Settings.IndexSettings
oMyIndexSettings.IndexMode = dd.e2DTableIndexModeFixed
oMyIndexSettings.IndexBegin = 500
oMyIndexSettings.IndexEnd = 600
oMyIndexSettings.IndexIncrement = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndexEnd_IRepTable2DIndexSettingsInt.htm`*
