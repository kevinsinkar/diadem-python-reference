---
title: "IRepSubSheetsInt"
description: "The SubSheets object provides the collection of all table sheets of an automatically increasing 2D table in DIAdem REPORT. A 2D table is automatically increasin"
---

# IRepSubSheetsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SubSheets

The SubSheets object provides the collection of all table sheets of an automatically increasing 2D table in DIAdem REPORT. A 2D table is automatically increasing if you select the value e2DTableIndexModeAutomaticallyIncreasing for the IndexMode for 2DTableIndexSettings property.

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
<p><a href="../../properties/irepsubsheetsint-subsheet/">Subsheet</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepsubsheetsint-recalculate/">Recalculate</a> | <a href="../../methods/irepsubsheetsint-reset/">Reset</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsheetint/">Sheet</a>.<a href="../../properties/irepsheetint-subsheets/">SubSheets</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSubSheetsInt.htm`*
