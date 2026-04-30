---
title: "IRepTable2DColumnTextInt.Settings"
description: "Specifies the properties of a 2D table column in which DIAdem REPORT displays a text from a text list."
---

# IRepTable2DColumnTextInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DTableColumnText

Specifies the properties of a 2D table column in which DIAdem REPORT displays a text from a text list.

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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnText)
oMyColumn.TextList(1).Text = "My text"
oMySettings = oMyColumn.Settings
oMySettings.Font.Bold = True
oMySettings.Alignment = dd.eTableAlignmentLeft
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepTable2DColumnTextInt.htm`*
