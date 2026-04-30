---
title: "IRepPositionInt.ByCoordinate"
description: "Uses the coordinates to specify the position of an object in DIAdem REPORT. Because you can use either the Bottom , Height , Left , Right , Top , and Width for "
---

# IRepPositionInt.ByCoordinate

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ByCoordinate for ObjectPosition

Uses the coordinates to specify the position of an object in DIAdem REPORT. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

## Signature

```python
return_value = obj.ByCoordinate
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

*Source: `ReportApi/properties/Report_property_ByCoordinate_IRepPositionInt.htm`*
