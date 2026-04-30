---
title: "IRepComFormulaSubArrowInt.Line"
description: "Specifies the line properties of a comment arrow or a formula graphic in DIAdem REPORT."
---

# IRepComFormulaSubArrowInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for ArrowElement

Specifies the line properties of a comment arrow or a formula graphic in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyArrow")
oMyPosComment = oMyComment.Position.ByCoordinate
oMyPosComment.X1 = 10
oMyPosComment.X2 = 30
oMyPosComment.Y1 = 10
oMyPosComment.Y2 = 30
oMyArrow = oMyComment.Arrow
oMyArrow.ArrowHeadAtBegin = dd.eArrowHeadNone
oMyArrow.ArrowHeadAtEnd = dd.eArrowHeadStandardArrow
oMyPosArrow = oMyArrow.Position
oMyPosArrow.XStart = 100
oMyPosArrow.XEnd = 40
oMyPosArrow.YStart = 100
oMyPosArrow.YEnd = 40
oMyArrow.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyArrow.Line.LineType = dd.eLineTypeSolid
oMyArrow.Line.Width = dd.eLineWidth0070
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepComFormulaSubArrowInt.htm`*
