---
title: "IRepTable2DGridLineInt"
description: "The 2DTableGridLine object provides the grid line properties of a 2D table in DIAdem REPORT."
---

# IRepTable2DGridLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableGridLine

The 2DTableGridLine object provides the grid line properties of a 2D table in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMySettings = oMy2DTable.Settings
oMySettings.UseXDoubleLine = False
oMySettings.UseYDoubleLine = False
oMySettings.BorderLineColor.SetPredefinedColor(dd.eColorIndexNone)
oMyGridHorSettings = oMy2DTable.Settings.GridHorizontal
oMyGridHorSettings.Visible = False
oMyGridVerSettings = oMy2DTable.Settings.GridVertical
oMyGridVerSettings.Visible = False
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dgridlineint-color/">Color</a> | <a href="../../properties/ireptable2dgridlineint-visible/">Visible</a> | <a href="../../properties/ireptable2dgridlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-gridhorizontal/">GridHorizontal</a> | <a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-gridvertical/">GridVertical</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DGridLineInt.htm`*
