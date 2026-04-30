---
title: "IRepD3AxisInt"
description: "The 3DAxisSystem object provides a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAxisSystem

The 3DAxisSystem object provides a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = dd.e3DDataStructureMatrix
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3axisint-axislist/">AxisList</a> | <a href="../../properties/irepd3axisint-colorlegend/">ColorLegend</a> | <a href="../../properties/irepd3axisint-curvelegend/">CurveLegend</a> | <a href="../../properties/irepd3axisint-curves3d/">Curves3D</a> | <a href="../../properties/irepd3axisint-index/">Index</a> | <a href="../../properties/irepd3axisint-isselected/">IsSelected</a> | <a href="../../properties/irepd3axisint-name/">Name</a> | <a href="../../properties/irepd3axisint-objecttype/">ObjectType</a> | <a href="../../properties/irepd3axisint-position/">Position</a> | <a href="../../properties/irepd3axisint-selectedelements/">SelectedElements</a> | <a href="../../properties/irepd3axisint-settings/">Settings</a> | <a href="../../properties/irepd3axisint-tagstored/">TagStored</a> | <a href="../../properties/irepd3axisint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd3axisint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepd3axisint-select/">Select</a> | <a href="../../methods/irepd3axisint-showpropertiesdlg/">ShowPropertiesDlg</a> | <a href="../../methods/irepd3axisint-updatescaling/">UpdateScaling</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcustomscalingaxissystem3dcontextint/">CustomScalingAxisSystem3DContext</a>.<a href="../../properties/irepcustomscalingaxissystem3dcontextint-axissystem/">AxisSystem</a> | <a href="../irepd3axisdropcontextint/">D3AxisSystemDropContext</a>.<a href="../../properties/irepd3axisdropcontextint-axissystem/">AxisSystem</a> | <a href="../irepd3curvedrawingcontextint/">D3CurveDrawingContext</a>.<a href="../../properties/irepd3curvedrawingcontextint-axissystem/">AxisSystem</a> | <a href="../irepd3curvetransformingcontextint/">D3CurveTransformingContext</a>.<a href="../../properties/irepd3curvetransformingcontextint-axissystem/">AxisSystem</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltip3daxiscontextint/">ToolTip3DAxisContext</a>.<a href="../../properties/ireptooltip3daxiscontextint-axissystem3d/">AxisSystem3D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3AxisInt.htm`*
