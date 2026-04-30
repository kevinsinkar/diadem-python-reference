---
title: "IRepPositionCoordinatesInt.Height"
description: "Specifies, in DIAdem REPORT, the height of an object as a percentage of the page area, in cm or in inch, if you position the object using the coordinate of one "
---

# IRepPositionCoordinatesInt.Height

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Height for ObjectPositionDefinedByCoordinates

Specifies, in DIAdem REPORT, the height of an object as a percentage of the page area, in cm or in inch, if you position the object using the coordinate of one corner, the height, and the width. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

## Signature

```python
obj.Height
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Height_IRepPositionCoordinatesInt.htm`*
