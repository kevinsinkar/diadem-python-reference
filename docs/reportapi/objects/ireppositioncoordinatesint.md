---
title: "IRepPositionCoordinatesInt"
description: "The ObjectPositionDefinedByCoordinates object provides the coordinates for the position of the object in DIAdem REPORT. Because you can use either the Bottom , "
---

# IRepPositionCoordinatesInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ObjectPositionDefinedByCoordinates

The ObjectPositionDefinedByCoordinates object provides the coordinates for the position of the object in DIAdem REPORT. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

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
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyPosFrame = oMyFrame.Position.ByCoordinate
oMyPosFrame.X1 = 40
oMyPosFrame.Width = 20
oMyPosFrame.Y1 = 10
oMyPosFrame.Height = 15
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppositioncoordinatesint-height/">Height</a> | <a href="../../properties/ireppositioncoordinatesint-width/">Width</a> | <a href="../../properties/ireppositioncoordinatesint-x1/">X1</a> | <a href="../../properties/ireppositioncoordinatesint-x2/">X2</a> | <a href="../../properties/ireppositioncoordinatesint-y1/">Y1</a> | <a href="../../properties/ireppositioncoordinatesint-y2/">Y2</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppositionint/">ObjectPosition</a>.<a href="../../properties/ireppositionint-bycoordinate/">ByCoordinate</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPositionCoordinatesInt.htm`*
