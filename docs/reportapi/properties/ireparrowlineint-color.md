---
title: "IRepArrowLineInt.Color"
description: "Specifies the color of an arrow line in DIAdem REPORT."
---

# IRepArrowLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for ArrowLine

Specifies the color of an arrow line in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

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

oMyArrow.ExportToImage("D:\\MyArrow",dd.eImageExportTypePNG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepArrowLineInt.htm`*
