---
title: "IRepArrowInt.ArrowHeadAtEnd"
description: "Specifies which arrow tip DIAdem REPORT plots at the end of an arrow."
---

# IRepArrowInt.ArrowHeadAtEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ArrowHeadAtEnd for Arrow

Specifies which arrow tip DIAdem REPORT plots at the end of an arrow.

## Signature

```python
obj.ArrowHeadAtEnd
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
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow,"MyArrow")

oMyArrow.ArrowHeadAtBegin = dd.eArrowHeadPoint
oMyArrow.ArrowHeadAtEnd = dd.eArrowHeadStandardArrow

oMyArrowPosition = oMyArrow.Position.ByCoordinate
oMyArrowPosition.X1 = 10
oMyArrowPosition.X2 = 40
oMyArrowPosition.Y1 = 30
oMyArrowPosition.Y2 = 90

oMyArrowLine = oMyArrow.Line
oMyArrowLine.LineType = dd.eLineTypeDotted
oMyArrowLine.Width = dd.eLineWidth0200

oMyArrowLineColor = oMyArrowLine.Color
oMyArrowLineColor.SetPredefinedColor(dd.eColorIndexGreen)

oMyArrow.ExportToImage(dd.LayoutWritePath + "MyNewArrow", dd.eImageExportTypePNG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ArrowHeadAtEnd_IRepArrowInt.htm`*
