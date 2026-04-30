---
title: "IRepTable2DInt"
description: "The 2DTable object provides a 2D table in DIAdem REPORT."
---

# IRepTable2DInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTable

The 2DTable object provides a 2D table in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dint-columns/">Columns</a> | <a href="../../properties/ireptable2dint-index/">Index</a> | <a href="../../properties/ireptable2dint-isselected/">IsSelected</a> | <a href="../../properties/ireptable2dint-name/">Name</a> | <a href="../../properties/ireptable2dint-objecttype/">ObjectType</a> | <a href="../../properties/ireptable2dint-position/">Position</a> | <a href="../../properties/ireptable2dint-selectedelements/">SelectedElements</a> | <a href="../../properties/ireptable2dint-settings/">Settings</a> | <a href="../../properties/ireptable2dint-tagstored/">TagStored</a> | <a href="../../properties/ireptable2dint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable2dint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireptable2dint-select/">Select</a> | <a href="../../methods/ireptable2dint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dcolumndrawingcontextint/">2DTableColumnDrawingContext</a>.<a href="../../properties/ireptable2dcolumndrawingcontextint-table/">Table</a> | <a href="../ireptable2ddrawingcellcontextint/">2DTableDrawingCellContext</a>.<a href="../../properties/ireptable2ddrawingcellcontextint-table/">Table</a> | <a href="../ireptable2ddrawingheaderfootercellcontextint/">2DTableDrawingHeaderFooterCellContext</a>.<a href="../../properties/ireptable2ddrawingheaderfootercellcontextint-table/">Table</a> | <a href="../ireptable2ddropcontextint/">2DTableDropContext</a>.<a href="../../properties/ireptable2ddropcontextint-table/">Table</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptable2dcolumntransformingcontextint/">Table2DColumnTransformingContext</a>.<a href="../../properties/ireptable2dcolumntransformingcontextint-table/">Table</a> | <a href="../ireptooltip2dtablecontextint/">ToolTip2DTableContext</a>.<a href="../../properties/ireptooltip2dtablecontextint-table2d/">Table2D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DInt.htm`*
