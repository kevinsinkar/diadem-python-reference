---
title: "IRepPositionInt"
description: "The ObjectPosition object provides the position of objects in DIAdem REPORT. Because you can use either the Bottom , Height , Left , Right , Top , and Width for"
---

# IRepPositionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ObjectPosition

The ObjectPosition object provides the position of objects in DIAdem REPORT. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

## Python example

```python
dd.Report.NewLayout()
oMyFormula = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFormulaDisplay ,"MyFormular")
oMyPosFormula = oMyFormula.Position.ByCoordinate
oMyFormula.Text = "a^2+b^2=c^2"
oMyPosFormula.X1 = 10
oMyPosFormula.X2 = 30
oMyPosFormula.Y1 = 10
oMyPosFormula.Y2 = 25
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppositionint-byborder/">ByBorder</a> | <a href="../../properties/ireppositionint-bycoordinate/">ByCoordinate</a> | <a href="../../properties/ireppositionint-zorder/">ZOrder</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-position/">Position</a> | <a href="../ireptable2dint/">2DTable</a>.<a href="../../properties/ireptable2dint-position/">Position</a> | <a href="../irepd3axisint/">3DAxisSystem</a>.<a href="../../properties/irepd3axisint-position/">Position</a> | <a href="../ireptable3dint/">3DTable</a>.<a href="../../properties/ireptable3dint-position/">Position</a> | <a href="../ireparrowint/">Arrow</a>.<a href="../../properties/ireparrowint-position/">Position</a> | <a href="../irepcircleint/">Circle</a>.<a href="../../properties/irepcircleint-position/">Position</a> | <a href="../irepcommentint/">Comment</a>.<a href="../../properties/irepcommentint-position/">Position</a> | <a href="../irepformuladisplayint/">FormulaDisplay</a>.<a href="../../properties/irepformuladisplayint-position/">Position</a> | <a href="../irepfreeframeint/">Frame</a>.<a href="../../properties/irepfreeframeint-position/">Position</a> | <a href="../irepimageint/">Image</a>.<a href="../../properties/irepimageint-position/">Position</a> | <a href="../ireppiechartint/">PieChart</a>.<a href="../../properties/ireppiechartint-position/">Position</a> | <a href="../ireppolarint/">PolarSystem</a>.<a href="../../properties/ireppolarint-position/">Position</a> | <a href="../ireptextobjectint/">RTFText</a>.<a href="../../properties/ireptextobjectint-position/">Position</a> | <a href="../irepspiderint/">Spider</a>.<a href="../../properties/irepspiderint-position/">Position</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPositionInt.htm`*
