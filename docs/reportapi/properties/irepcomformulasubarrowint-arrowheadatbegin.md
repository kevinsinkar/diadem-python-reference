---
title: "IRepComFormulaSubArrowInt.ArrowHeadAtBegin"
description: "Specifies the type of arrowhead at the beginning of an arrow of a comment or a formula graphic in DIAdem REPORT."
---

# IRepComFormulaSubArrowInt.ArrowHeadAtBegin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ArrowHeadAtBegin for ArrowElement

Specifies the type of arrowhead at the beginning of an arrow of a comment or a formula graphic in DIAdem REPORT.

## Signature

```python
obj.ArrowHeadAtBegin
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eArrowHeadNone` | 0 | No arrow |
| `eArrowHeadStandardArrow` | 1 | Standard arrow |
| `eArrowHeadNormArrow` | 2 | Norm arrow |
| `eArrowHeadPoint` | 3 | Arrow with point |

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
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ArrowHeadAtBegin_IRepComFormulaSubArrowInt.htm`*
