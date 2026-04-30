---
title: "IRepPolarInt"
description: "The PolarAxisSystem object provides a polar axis system in DIAdem REPORT."
---

# IRepPolarInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarSystem

The PolarAxisSystem object provides a polar axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarint-curvelegend/">CurveLegend</a> | <a href="../../properties/ireppolarint-curvespolar/">CurvesPolar</a> | <a href="../../properties/ireppolarint-index/">Index</a> | <a href="../../properties/ireppolarint-isselected/">IsSelected</a> | <a href="../../properties/ireppolarint-name/">Name</a> | <a href="../../properties/ireppolarint-objecttype/">ObjectType</a> | <a href="../../properties/ireppolarint-position/">Position</a> | <a href="../../properties/ireppolarint-radialaxis/">RadialAxis</a> | <a href="../../properties/ireppolarint-sectors/">Sectors</a> | <a href="../../properties/ireppolarint-selectedelements/">SelectedElements</a> | <a href="../../properties/ireppolarint-settings/">Settings</a> | <a href="../../properties/ireppolarint-tagstored/">TagStored</a> | <a href="../../properties/ireppolarint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppolarint-convertpagexypositiontoangle/">ConvertPageXYPositionToAngle</a> | <a href="../../methods/ireppolarint-convertpagexypositiontolength/">ConvertPageXYPositionToLength</a> | <a href="../../methods/ireppolarint-convertpolarcoordinatetopagexposition/">ConvertPolarCoordinateToPageXPosition</a> | <a href="../../methods/ireppolarint-convertpolarcoordinatetopageyposition/">ConvertPolarCoordinateToPageYPosition</a> | <a href="../../methods/ireppolarint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireppolarint-select/">Select</a> | <a href="../../methods/ireppolarint-showpropertiesdlg/">ShowPropertiesDlg</a> | <a href="../../methods/ireppolarint-updatescaling/">UpdateScaling</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolaraxissystemclickedwithkeycontextint/">PolarAxisSystemClickedWithKeyContext</a>.<a href="../../properties/ireppolaraxissystemclickedwithkeycontextint-axissystempolar/">AxisSystemPolar</a> | <a href="../ireppolarcurvedrawingcontextint/">PolarCurveDrawingContext</a>.<a href="../../properties/ireppolarcurvedrawingcontextint-polarsystem/">PolarSystem</a> | <a href="../ireppolardropcontextint/">PolarSystemDropContext</a>.<a href="../../properties/ireppolardropcontextint-polarsystem/">PolarSystem</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltippolarcontextint/">ToolTipPolarContext</a>.<a href="../../properties/ireptooltippolarcontextint-polar/">Polar</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarInt.htm`*
