---
title: "IRepTable2DColumnExpressionInt.Settings"
description: "Specifies the properties of a 2D table column in which DIAdem REPORT displays a DIAdem expression."
---

# IRepTable2DColumnExpressionInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DTableColumnExpression

Specifies the properties of a 2D table column in which DIAdem REPORT displays a DIAdem expression.

## Signature

```python
return_value = obj.Settings
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
oMy2DTable.Settings.Header.Height = 20
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnExpression)
oMyColumn.Expression = "@@CurrDate@@, @@CurrTime@@"
oMyColumn.Settings.Font.Bold = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepTable2DColumnExpressionInt.htm`*
