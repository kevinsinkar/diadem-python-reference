---
title: "IRepTable2DBackgroundColors"
description: "The 2DTableItemBackgroundColor object provides properties for the display of a 2D table."
---

# IRepTable2DBackgroundColors

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableItemBackgroundColor

The 2DTableItemBackgroundColor object provides properties for the display of a 2D table.

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
oMyRow = oMy2DTable.Settings.RowBackground
oMyRow.BackgroundColor.ColorIndex = dd.eColorIndexGrey
oMyRow.AlternatingBackgroundColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dbackgroundcolors-alternatingbackgroundcolor/">AlternatingBackgroundColor</a> | <a href="../../properties/ireptable2dbackgroundcolors-backgroundcolor/">BackgroundColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-columnbackground/">ColumnBackground</a> | <a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-rowbackground/">RowBackground</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DBackgroundColors.htm`*
