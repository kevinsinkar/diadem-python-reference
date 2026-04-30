---
title: "IRepSubSheetInt"
description: "The SubSheets object provides a table sheet of an automatically increasing 2D table in DIAdem REPORT. A 2D table is automatically increasing if you select the v"
---

# IRepSubSheetInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SubSheet

The SubSheets object provides a table sheet of an automatically increasing 2D table in DIAdem REPORT. A 2D table is automatically increasing if you select the value e2DTableIndexModeAutomaticallyIncreasing for the IndexMode for 2DTableIndexSettings property.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsubsheetint-count/">Count</a> | <a href="../../properties/irepsubsheetint-index/">Index</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsubsheetsint/">SubSheets</a>.<a href="../../properties/irepsubsheetsint-subsheet/">Subsheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSubSheetInt.htm`*
