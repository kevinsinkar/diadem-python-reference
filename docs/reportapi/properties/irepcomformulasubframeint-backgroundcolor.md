---
title: "IRepComFormulaSubFrameInt.BackgroundColor"
description: "Specifies the background color of the frame of a formula graphic in DIAdem REPORT."
---

# IRepComFormulaSubFrameInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for FrameElement

Specifies the background color of the frame of a formula graphic in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
```

## Python example

```python
dd.Report.NewLayout()
oMyFormula = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFormulaDisplay ,"MyFormular")
oMyPosFormula = oMyFormula.Position.ByCoordinate
oMyFormula.Text = "a^2+b^2=c^2"
oMyFormula.FontName = "Arial"
oMyFormula.FontColor.SetPredefinedColor(dd.ePredefinedColorDarkRed)
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepComFormulaSubFrameInt.htm`*
