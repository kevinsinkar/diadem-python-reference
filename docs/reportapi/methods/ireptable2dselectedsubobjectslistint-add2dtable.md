---
title: "IRepTable2DSelectedSubObjectsListInt.Add2DTable"
description: "Selects the subobject of a 2D table in DIAdem REPORT associated with a specific index."
---

# IRepTable2DSelectedSubObjectsListInt.Add2DTable

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add2DTable for 2DTableSelectedElements

Selects the subobject of a 2D table in DIAdem REPORT associated with a specific index.

## Signature

```python
return_value = obj.Add2DTable(ElementType, Index)
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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = dd.eTableAlignmentDecimalPoint
oMyColumn.Settings.Format = "d.dddd"
dd.Report.Refresh()
oMy2DTable.SelectedElements.Add2DTable(dd.e2DTableElementHeader, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add2DTable_IRepTable2DSelectedSubObjectsListInt.htm`*
