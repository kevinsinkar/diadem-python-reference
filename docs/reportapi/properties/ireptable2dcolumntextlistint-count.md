---
title: "IRepTable2DColumnTextListInt.Count"
description: "Returns the number of texts in a 2D table column in DIAdem REPORT."
---

# IRepTable2DColumnTextListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 2DTableColumnTextList

Returns the number of texts in a 2D table column in DIAdem REPORT.

## Signature

```python
obj.Count
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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnText)
oMyTextList = oMyColumn.TextList
oMyTextList.Count = 5
for I in range( 1, oMyTextList.Count+1):
    oMyTextList(I).Text = "Row " + I
oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticMinimum
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepTable2DColumnTextListInt.htm`*
