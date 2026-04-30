---
title: "IRepTable2DColumnChannelInt.Channel"
description: "Specifies the channel which DIAdem REPORT displays in the column of a 2D table."
---

# IRepTable2DColumnChannelInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 2DTableColumnChannel

Specifies the channel which DIAdem REPORT displays in the column of a 2D table.

## Signature

```python
return_value = obj.Channel
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
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepTable2DColumnChannelInt.htm`*
