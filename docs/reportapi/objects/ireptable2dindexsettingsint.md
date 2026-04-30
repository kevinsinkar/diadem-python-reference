---
title: "IRepTable2DIndexSettingsInt"
description: "The 2DTableIndexSettings object provides the scaling properties of a 2D table in DIAdem REPORT."
---

# IRepTable2DIndexSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableIndexSettings

The 2DTableIndexSettings object provides the scaling properties of a 2D table in DIAdem REPORT.

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
oMyIndexSettings.IndexBegin = 1
oMyIndexSettings.IndexEnd = 1024
oMyIndexSettings.IndexIncrement = 100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dindexsettingsint-indexbegin/">IndexBegin</a> | <a href="../../properties/ireptable2dindexsettingsint-indexend/">IndexEnd</a> | <a href="../../properties/ireptable2dindexsettingsint-indexincrement/">IndexIncrement</a> | <a href="../../properties/ireptable2dindexsettingsint-indexmode/">IndexMode</a> | <a href="../../properties/ireptable2dindexsettingsint-rowheight/">RowHeight</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-indexsettings/">IndexSettings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DIndexSettingsInt.htm`*
