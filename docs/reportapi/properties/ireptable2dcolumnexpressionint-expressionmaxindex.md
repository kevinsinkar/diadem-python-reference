---
title: "IRepTable2DColumnExpressionInt.ExpressionMaxIndex"
description: "Specifies the maximum number of table rows for variables or for DIAdem expressions in a 2D table in DIAdem REPORT. You can assign a numeric value or a DIAdem ex"
---

# IRepTable2DColumnExpressionInt.ExpressionMaxIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ExpressionMaxIndex for 2DTableColumnExpression

Specifies the maximum number of table rows for variables or for DIAdem expressions in a 2D table in DIAdem REPORT. You can assign a numeric value or a DIAdem expression to the ExpressionMaxIndex property.

## Signature

```python
obj.ExpressionMaxIndex
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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnExpression)
oMyColumn.Expression = "@@CurrTime@@"
oMyColumn.ExpressionMaxIndex = 1
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

*Source: `ReportApi/properties/Report_property_ExpressionMaxIndex_IRepTable2DColumnExpressionInt.htm`*
