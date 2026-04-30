---
title: "IRepPositionBordersInt.Top"
description: "Specifies, in DIAdem REPORT, the distance from the upper edge of an object to the upper edge of the worksheet as a percentage of the page area, in cm or in inch"
---

# IRepPositionBordersInt.Top

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Top for ObjectPositionDefinedByBorders

Specifies, in DIAdem REPORT, the distance from the upper edge of an object to the upper edge of the worksheet as a percentage of the page area, in cm or in inch, if you use margins to position the object. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

## Signature

```python
obj.Top
```

## Python example

```python
dd.Report.NewLayout()
oMyFormula = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFormulaDisplay ,"MyFormular")
oMyPosFormula = oMyFormula.Position.ByBorder
oMyFormula.Text = "a^2+b^2=c^2"
oMyPosFormula.Left = 10
oMyPosFormula.Right = 70
oMyPosFormula.Bottom = 10
oMyPosFormula.Top = 75
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Top_IRepPositionBordersInt.htm`*
