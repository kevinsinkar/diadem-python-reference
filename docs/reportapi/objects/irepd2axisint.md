---
title: "IRepD2AxisInt"
description: "The 2DAxisSystem object provides a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisSystem

The 2DAxisSystem object provides a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisint-colorlegend/">ColorLegend</a> | <a href="../../properties/irepd2axisint-curvelegend/">CurveLegend</a> | <a href="../../properties/irepd2axisint-curves2d/">Curves2D</a> | <a href="../../properties/irepd2axisint-index/">Index</a> | <a href="../../properties/irepd2axisint-isselected/">IsSelected</a> | <a href="../../properties/irepd2axisint-name/">Name</a> | <a href="../../properties/irepd2axisint-objecttype/">ObjectType</a> | <a href="../../properties/irepd2axisint-position/">Position</a> | <a href="../../properties/irepd2axisint-selectedelements/">SelectedElements</a> | <a href="../../properties/irepd2axisint-settings/">Settings</a> | <a href="../../properties/irepd2axisint-tagstored/">TagStored</a> | <a href="../../properties/irepd2axisint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepd2axisint-xaxis/">XAxis</a> | <a href="../../properties/irepd2axisint-yaxis/">YAxis</a> | <a href="../../properties/irepd2axisint-yaxislist/">YAxisList</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2axisint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepd2axisint-select/">Select</a> | <a href="../../methods/irepd2axisint-showpropertiesdlg/">ShowPropertiesDlg</a> | <a href="../../methods/irepd2axisint-updatescaling/">UpdateScaling</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcustomscalingaxissystem2dcontextint/">CustomScalingAxisSystem2DContext</a>.<a href="../../properties/irepcustomscalingaxissystem2dcontextint-axissystem/">AxisSystem</a> | <a href="../irepcustomscalingaxissystem2dscaledcontextint/">CustomScalingAxisSystem2DScaledContext</a>.<a href="../../properties/irepcustomscalingaxissystem2dscaledcontextint-axissystem/">AxisSystem</a> | <a href="../irepd2axissystemclickedwithkeycontextint/">D2AxisSystemClickedWithKeyContext</a>.<a href="../../properties/irepd2axissystemclickedwithkeycontextint-axissystem2d/">AxisSystem2D</a> | <a href="../irepd2axisdropcontextint/">D2AxisSystemDropContext</a>.<a href="../../properties/irepd2axisdropcontextint-axissystem/">AxisSystem</a> | <a href="../irepd2curvedrawingcontextint/">D2CurveDrawingContext</a>.<a href="../../properties/irepd2curvedrawingcontextint-axissystem/">AxisSystem</a> | <a href="../irepd2curvetransformingcontextint/">D2CurveTransformingContext</a>.<a href="../../properties/irepd2curvetransformingcontextint-axissystem/">AxisSystem</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltip2daxiscontextint/">ToolTip2DAxisContext</a>.<a href="../../properties/ireptooltip2daxiscontextint-axissystem2d/">AxisSystem2D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisInt.htm`*
