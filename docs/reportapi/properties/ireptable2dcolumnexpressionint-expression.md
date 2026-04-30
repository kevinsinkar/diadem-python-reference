---
title: "IRepTable2DColumnExpressionInt.Expression"
description: "Specifies the DIAdem expression, whose value DIAdem REPORT displays in a cell of a 2D table."
---

# IRepTable2DColumnExpressionInt.Expression

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Expression for 2DTableColumnExpression

Specifies the DIAdem expression, whose value DIAdem REPORT displays in a cell of a 2D table.

## Signature

```python
obj.Expression
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

*Source: `ReportApi/properties/Report_property_Expression_IRepTable2DColumnExpressionInt.htm`*
