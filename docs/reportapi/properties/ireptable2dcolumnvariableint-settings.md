---
title: "IRepTable2DColumnVariableInt.Settings"
description: "Specifies the properties of a 2D table column in which DIAdem REPORT displays the contents of a variable."
---

# IRepTable2DColumnVariableInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DTableColumnVariable

Specifies the properties of a 2D table column in which DIAdem REPORT displays the contents of a variable.

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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnVariable)
oMyColumn.VariableName = "CurrTime"
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

*Source: `ReportApi/properties/Report_property_Settings_IRepTable2DColumnVariableInt.htm`*
