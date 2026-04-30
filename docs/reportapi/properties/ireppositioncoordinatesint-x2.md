---
title: "IRepPositionCoordinatesInt.X2"
description: "Specifies the distance between the right edge of an object and the left edge of the worksheet as a percentage of the page area, in cm or in inch. Because you ca"
---

# IRepPositionCoordinatesInt.X2

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: X2 for ObjectPositionDefinedByCoordinates

Specifies the distance between the right edge of an object and the left edge of the worksheet as a percentage of the page area, in cm or in inch. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

## Signature

```python
obj.X2
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_X2_IRepPositionCoordinatesInt.htm`*
