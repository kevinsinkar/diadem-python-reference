---
title: "IRepTable2DColumnChannelInt.UseExpansion"
description: "Specifies whether DIAdem displays the values of several channels if several channels with the same channel name exist in a 2D table column in DIAdem REPORT. You"
---

# IRepTable2DColumnChannelInt.UseExpansion

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseExpansion for 2DTableColumnChannel

Specifies whether DIAdem displays the values of several channels if several channels with the same channel name exist in a 2D table column in DIAdem REPORT. You must first enable the expansion mode .

## Signature

```python
obj.UseExpansion
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
oMyColumn.Channel.Reference = "*/Mean"
dd.Report.Settings.CurveExpansion.Enable = True
oMyColumn.UseExpansion = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseExpansion_IRepTable2DColumnChannelInt.htm`*
