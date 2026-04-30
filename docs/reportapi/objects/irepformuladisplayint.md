---
title: "IRepFormulaDisplayInt"
description: "The FormulaDisplay object provides a formula graphic in DIAdem REPORT."
---

# IRepFormulaDisplayInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: FormulaDisplay

The FormulaDisplay object provides a formula graphic in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyFormula = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFormulaDisplay ,"MyFormular")
oMyPosFormula = oMyFormula.Position.ByCoordinate
oMyFormula.Text = "a^2+b^2=c^2"
oMyPosFormula.X1 = 20
oMyPosFormula.X2 = 40
oMyPosFormula.Y1 = 20
oMyPosFormula.Y2 = 35
oMyArrow = oMyFormula.Arrow
oMyArrow.Line.Color.SetPredefinedColor(dd.ePredefinedColorDarkViolet)
oMyArrow.Line.LineType = dd.eLineTypeSolid
oMyArrow.Line.Width = dd.eLineWidth0100
oMyArrow.ArrowHeadAtBegin = dd.eArrowHeadNormArrow
oMyFrame = oMyFormula.Frame
oMyFrame.BorderLine.Color.SetPredefinedColor(dd.ePredefinedColorDarkGreen)
oMyFrame.BackgroundColor.SetPredefinedColor(dd.ePredefinedColorYellow)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepformuladisplayint-arrow/">Arrow</a> | <a href="../../properties/irepformuladisplayint-fontcolor/">FontColor</a> | <a href="../../properties/irepformuladisplayint-fontname/">FontName</a> | <a href="../../properties/irepformuladisplayint-frame/">Frame</a> | <a href="../../properties/irepformuladisplayint-index/">Index</a> | <a href="../../properties/irepformuladisplayint-isselected/">IsSelected</a> | <a href="../../properties/irepformuladisplayint-name/">Name</a> | <a href="../../properties/irepformuladisplayint-objecttype/">ObjectType</a> | <a href="../../properties/irepformuladisplayint-position/">Position</a> | <a href="../../properties/irepformuladisplayint-selectedelements/">SelectedElements</a> | <a href="../../properties/irepformuladisplayint-tagstored/">TagStored</a> | <a href="../../properties/irepformuladisplayint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepformuladisplayint-text/">Text</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepformuladisplayint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepformuladisplayint-select/">Select</a> | <a href="../../methods/irepformuladisplayint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltipformuladisplaycontextint/">ToolTipFormulaDisplayContext</a>.<a href="../../properties/ireptooltipformuladisplaycontextint-formuladisplay/">FormulaDisplay</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepFormulaDisplayInt.htm`*
