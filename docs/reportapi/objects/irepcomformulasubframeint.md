---
title: "IRepComFormulaSubFrameInt"
description: "The FrameElement object provides the frame for a formula graphic in DIAdem REPORT."
---

# IRepComFormulaSubFrameInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: FrameElement

The FrameElement object provides the frame for a formula graphic in DIAdem REPORT.

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
<p><a href="../../properties/irepcomformulasubframeint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepcomformulasubframeint-borderline/">BorderLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepformuladisplayint/">FormulaDisplay</a>.<a href="../../properties/irepformuladisplayint-frame/">Frame</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepComFormulaSubFrameInt.htm`*
