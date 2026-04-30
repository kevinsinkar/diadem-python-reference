---
title: "IRepComFormulaSubArrowPositionInt.UseSnappedArrowHead"
description: "Specifies whether DIAdem REPORT maintains the current position of the arrow end when you move the objects."
---

# IRepComFormulaSubArrowPositionInt.UseSnappedArrowHead

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseSnappedArrowHead for ArrowElementPosition

Specifies whether DIAdem REPORT maintains the current position of the arrow end when you move the objects.

## Signature

```python
obj.UseSnappedArrowHead
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
oMyPosArrow.UseSnappedArrowHead = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseSnappedArrowHead_IRepComFormulaSubArrowPositionInt.htm`*
