---
title: "IRepTable2DColumnExpressionInt"
description: "The 2DTableColumnExpression object provides a 2D table column in DIAdem REPORT. This table column takes its contents from a DIAdem expression."
---

# IRepTable2DColumnExpressionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnExpression

The 2DTableColumnExpression object provides a 2D table column in DIAdem REPORT. This table column takes its contents from a DIAdem expression.

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
oMyColumn.Settings.Font.Color.SetpredefinedColor(dd.ePredefinedColorBlue)
oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticMinimum
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnexpressionint-expression/">Expression</a> | <a href="../../properties/ireptable2dcolumnexpressionint-expressionmaxindex/">ExpressionMaxIndex</a> | <a href="../../properties/ireptable2dcolumnexpressionint-index/">Index</a> | <a href="../../properties/ireptable2dcolumnexpressionint-settings/">Settings</a> | <a href="../../properties/ireptable2dcolumnexpressionint-tagstored/">TagStored</a> | <a href="../../properties/ireptable2dcolumnexpressionint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireptable2dcolumnexpressionint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-add/">Add</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-changetype/">ChangeType</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-copy/">Copy</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-item/">Item</a> | <a href="../ireptable2dcolumntransformingcontextint/">Table2DColumnTransformingContext</a>.<a href="../../properties/ireptable2dcolumntransformingcontextint-column/">Column</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnExpressionInt.htm`*
