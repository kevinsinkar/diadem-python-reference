---
title: "IRepPositionBordersInt"
description: "The ObjectPositionDefinedByBorders object provides the distances for the position of the object in DIAdem REPORT. Because you can use either the Bottom , Height"
---

# IRepPositionBordersInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ObjectPositionDefinedByBorders

The ObjectPositionDefinedByBorders object provides the distances for the position of the object in DIAdem REPORT. Because you can use either the Bottom , Height , Left , Right , Top , and Width for the ObjectPositionDefinedByBorders property, or the Height , Width , X1 , X2 , Y1 , and Y2 for the ObjectPositionDefinedByCoordinates property to specify the position, these properties impact each other and the value of the property set first can be modified by another property.

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
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyPosFrame = oMyFrame.Position.ByBorder
oMyPosFrame.Left = 40
oMyPosFrame.Width = 20
oMyPosFrame.Bottom = 10
oMyPosFrame.Height = 15
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppositionbordersint-bottom/">Bottom</a> | <a href="../../properties/ireppositionbordersint-height/">Height</a> | <a href="../../properties/ireppositionbordersint-left/">Left</a> | <a href="../../properties/ireppositionbordersint-right/">Right</a> | <a href="../../properties/ireppositionbordersint-top/">Top</a> | <a href="../../properties/ireppositionbordersint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppositionint/">ObjectPosition</a>.<a href="../../properties/ireppositionint-byborder/">ByBorder</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPositionBordersInt.htm`*
