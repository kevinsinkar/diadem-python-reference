---
title: "IRepComFormulaSubArrowInt"
description: "The ArrowElement object provides the comment arrow and a formula graphic in DIAdem REPORT."
---

# IRepComFormulaSubArrowInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ArrowElement

The ArrowElement object provides the comment arrow and a formula graphic in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcomformulasubarrowint-arrowheadatbegin/">ArrowHeadAtBegin</a> | <a href="../../properties/irepcomformulasubarrowint-arrowheadatend/">ArrowHeadAtEnd</a> | <a href="../../properties/irepcomformulasubarrowint-line/">Line</a> | <a href="../../properties/irepcomformulasubarrowint-position/">Position</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcommentint/">Comment</a>.<a href="../../properties/irepcommentint-arrow/">Arrow</a> | <a href="../irepformuladisplayint/">FormulaDisplay</a>.<a href="../../properties/irepformuladisplayint-arrow/">Arrow</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepComFormulaSubArrowInt.htm`*
