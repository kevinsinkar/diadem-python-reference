---
title: "2DTableColumnTextList"
description: "Collection of all Table2DColumnTextItem objects in DIAdem REPORT. Use the 2DTableColumnTextList collection to access a text from a 2D table column in DIAdem REP"
---

# 2DTableColumnTextList

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DTableColumnTextList

Collection of all Table2DColumnTextItem objects in DIAdem REPORT. Use the 2DTableColumnTextList collection to access a text from a 2D table column in DIAdem REPORT. This table column takes its contents from a text list.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnText)
oMyTextList = oMyColumn.TextList
oMyTextList.Count = 5
for I in range( 1, oMyTextList.Count+1):
    oMyTextList(I).Text = "Row " + I
oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticMinimum
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumntextlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable2dcolumntextlistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireptable2dcolumntextint/">2DTableColumnText</a>.<a href="../../properties/ireptable2dcolumntextint-textlist/">TextList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnTextListInt.htm`*
