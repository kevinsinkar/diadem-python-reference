---
title: "IRepPieChartInt"
description: "The PieChart object provides a pie chart in DIAdem REPORT."
---

# IRepPieChartInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChart

The PieChart object provides a pie chart in DIAdem REPORT.

## Python example

```python
oPieChart = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "PieChart1")
```

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMyPieChart = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "MyPieChart")
oMyPos = oMyPieChart.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurvePieChart = oMyPieChart.CurvePieChart # CurvePieChartPieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartint-curvepiechart/">CurvePieChart</a> | <a href="../../properties/ireppiechartint-index/">Index</a> | <a href="../../properties/ireppiechartint-isselected/">IsSelected</a> | <a href="../../properties/ireppiechartint-legend/">Legend</a> | <a href="../../properties/ireppiechartint-name/">Name</a> | <a href="../../properties/ireppiechartint-objecttype/">ObjectType</a> | <a href="../../properties/ireppiechartint-position/">Position</a> | <a href="../../properties/ireppiechartint-selectedelements/">SelectedElements</a> | <a href="../../properties/ireppiechartint-settings/">Settings</a> | <a href="../../properties/ireppiechartint-tagstored/">TagStored</a> | <a href="../../properties/ireppiechartint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppiechartint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireppiechartint-select/">Select</a> | <a href="../../methods/ireppiechartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltippiechartcontextint/">ToolTipPieChartContext</a>.<a href="../../properties/ireptooltippiechartcontextint-piechart/">PieChart</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartInt.htm`*
