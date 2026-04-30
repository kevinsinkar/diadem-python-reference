---
title: "IRepComFormulaSubArrowPositionInt.XEnd"
description: "Specifies the horizontal distance of the arrow tip from the left bottom corner of a comment or a formula graphic in DIAdem REPORT. Specify the distance as a per"
---

# IRepComFormulaSubArrowPositionInt.XEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XEnd for ArrowElementPosition

Specifies the horizontal distance of the arrow tip from the left bottom corner of a comment or a formula graphic in DIAdem REPORT. Specify the distance as a percentage of the worksheet size.

## Signature

```python
obj.XEnd
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XEnd_IRepComFormulaSubArrowPositionInt.htm`*
