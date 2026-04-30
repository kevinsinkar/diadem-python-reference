---
title: "IRepFormulaDisplayInt.Position"
description: "Specifies the position of a formula graphic in a DIAdem REPORT worksheet."
---

# IRepFormulaDisplayInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for FormulaDisplay

Specifies the position of a formula graphic in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
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

*Source: `ReportApi/properties/Report_property_Position_IRepFormulaDisplayInt.htm`*
