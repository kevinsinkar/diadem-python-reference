---
title: "IRepArrowLineInt"
description: "The ArrowLine object provides the arrow line in DIAdem REPORT."
---

# IRepArrowLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ArrowLine

The ArrowLine object provides the arrow line in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow,"MyArrow")
oMyArrowLine = oMyArrow.Line
dd.MsgBoxDisp(oMyArrowLine.Width)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireparrowlineint-color/">Color</a> | <a href="../../properties/ireparrowlineint-linetype/">LineType</a> | <a href="../../properties/ireparrowlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcommentarrowadditionalint/">AdditionalCommentArrow</a>.<a href="../../properties/irepcommentarrowadditionalint-line/">Line</a> | <a href="../ireparrowint/">Arrow</a>.<a href="../../properties/ireparrowint-line/">Line</a> | <a href="../irepcomformulasubarrowint/">ArrowElement</a>.<a href="../../properties/irepcomformulasubarrowint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepArrowLineInt.htm`*
