---
title: "IRepSubSheetsInt.Recalculate"
description: "Recalculates the number of table sheets of an automatically increasing 2D table in DIAdem REPORT. After replotting the report, DIAdem also recalculates the numb"
---

# IRepSubSheetsInt.Recalculate

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Recalculate for SubSheets

Recalculates the number of table sheets of an automatically increasing 2D table in DIAdem REPORT. After replotting the report, DIAdem also recalculates the number of table pages.

## Signature

```python
obj.Recalculate()
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
oMySubSheets.Recalculate()
print("Number of subsheets: " + oMySubSheets.Subsheet.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Recalculate_IRepSubSheetsInt.htm`*
