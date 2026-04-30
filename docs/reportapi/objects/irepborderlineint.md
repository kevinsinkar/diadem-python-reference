---
title: "IRepBorderLineInt"
description: "The BorderLine object provides the properties of the frame line of a comment, circle, or rectangle in DIAdem REPORT."
---

# IRepBorderLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: BorderLine

The BorderLine object provides the properties of the frame line of a comment, circle, or rectangle in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyBackgroundColor = oMyFrame.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyBackgroundColor.Transparency = 50
oMyPosition = oMyFrame.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 50
oMyPosition.Y2 = 80
oMyBorderLine = oMyFrame.BorderLine
oMyBorderLine.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMyBorderLine.LineType = dd.eLineTypeDotted
oMyBorderLine.Width = dd.eLineWidth0140
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepborderlineint-color/">Color</a> | <a href="../../properties/irepborderlineint-linetype/">LineType</a> | <a href="../../properties/irepborderlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcommenttextadditionalint/">AdditionalCommentText</a>.<a href="../../properties/irepcommenttextadditionalint-borderline/">BorderLine</a> | <a href="../irepcomformulasubframeint/">FrameElement</a>.<a href="../../properties/irepcomformulasubframeint-borderline/">BorderLine</a> | <a href="../irepframelineint/">FrameLine</a>.<a href="../../properties/irepframelineint-linebottom/">LineBottom</a> | <a href="../irepframelineint/">FrameLine</a>.<a href="../../properties/irepframelineint-lineleft/">LineLeft</a> | <a href="../irepframelineint/">FrameLine</a>.<a href="../../properties/irepframelineint-lineright/">LineRight</a> | <a href="../irepframelineint/">FrameLine</a>.<a href="../../properties/irepframelineint-linetop/">LineTop</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepBorderLineInt.htm`*
