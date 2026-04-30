---
title: "IRepFormulaDisplaySelectedSubObjectsListInt.AddFormulaDisplay"
description: "Selects the subobject of a formula graphic in DIAdem REPORT associated with a specific index."
---

# IRepFormulaDisplaySelectedSubObjectsListInt.AddFormulaDisplay

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: AddFormulaDisplay for FormulaDisplaySelectedElements

Selects the subobject of a formula graphic in DIAdem REPORT associated with a specific index.

## Signature

```python
return_value = obj.AddFormulaDisplay(ElementType, Index)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCommentElementArrow` | 0 | Arrow |
| `eCommentFrameTop` | 1 | Upper frame |
| `eCommentFrameBottom` | 2 | Lower frame |
| `eCommentFrameLeft` | 3 | Left frame |
| `eCommentFrameRight` | 4 | Right frame |

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
oMyFormula.SelectedElements.AddFormulaDisplay(dd.eCommentElementArrow, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_AddFormulaDisplay_IRepFormulaDisplaySelectedSubObjectsListInt.htm`*
