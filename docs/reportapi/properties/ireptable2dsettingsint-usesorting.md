---
title: "IRepTable2DSettingsInt.UseSorting"
description: "Specifies whether DIAdem REPORT sorts the values in the columns of a table. If you want to both specify the value e2DTableColumnExpression for Type for 2DTableC"
---

# IRepTable2DSettingsInt.UseSorting

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseSorting for 2DTableSettings

Specifies whether DIAdem REPORT sorts the values in the columns of a table. If you want to both specify the value e2DTableColumnExpression for Type for 2DTableColumn and sort the data, you must also specify the property ExpressionMaxIndex for 2DTableColumnExpression . For example, if you want to sort the output of the channel names of the first channel group, specify @@Data.Root.ChannelGroups(1).Channels(D2TabRow)@@ as the DIAdem expression and assign the DIAdem expression @@Data.Root.ChannelGroups(1).Channels.Count@@ to the ExpressionMaxIndex property for 2DTableColumnExpression.

## Signature

```python
obj.UseSorting
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

*Source: `ReportApi/properties/Report_property_UseSorting_IRepTable2DSettingsInt.htm`*
