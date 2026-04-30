---
title: "IRepSubSheetsInt.Reset"
description: "Resets the number of table sheets of an automatically increasing 2D table in DIAdem REPORT. DIAdem replots the report or calls the Recalculate for SubSheets met"
---

# IRepSubSheetsInt.Reset

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Reset for SubSheets

Resets the number of table sheets of an automatically increasing 2D table in DIAdem REPORT. DIAdem replots the report or calls the Recalculate for SubSheets method to recalculate the number of table sheets.

## Signature

```python
obj.Reset()
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
oMyIndexSettings = oMy2DTable.Settings.IndexSettings
oMyIndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticallyIncreasing
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[1]"
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMySubSheets = dd.Report.ActiveSheet.SubSheets
if dd.DataChanged :
    oMySubSheets.Reset()
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Reset_IRepSubSheetsInt.htm`*
