---
title: "IRepTable2DColumnSettingsInt.SortOrder"
description: "Specifies in which order DIAdem REPORT sorts the values in the columns of a table."
---

# IRepTable2DColumnSettingsInt.SortOrder

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SortOrder for 2DTableColumnSettings

Specifies in which order DIAdem REPORT sorts the values in the columns of a table.

## Signature

```python
obj.SortOrder
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTableSortOrderUp` | 0 | Ascending |
| `eTableSortOrderDown` | 1 | Descending |
| `eTableSortNoOrder` | 2 | Include in sort |
| `eTableNoSort` | 3 | Do not sort |

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMy2DTableColumns = oMy2DTable.Columns
oMyColumn1 = oMy2DTableColumns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTableColumns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
oMyColumn3 = oMy2DTableColumns.Add(dd.e2DTableColumnChannel)
oMyColumn3.Channel.Reference = "[1]/[3]"

oMy2DTable.Settings.UseSorting = True
oMyColumn2.Settings.SortOrder = dd.eTableSortOrderDown
oMyColumn3.Settings.SortOrder = dd.eTableSortNoOrder
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SortOrder_IRepTable2DColumnSettingsInt.htm`*
