---
title: "IRepFrameLineInt"
description: "The FrameLine object provides the properties of the frame line of a comment, circle, or rectangle in DIAdem REPORT."
---

# IRepFrameLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: FrameLine

The FrameLine object provides the properties of the frame line of a comment, circle, or rectangle in DIAdem REPORT.

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
<p><a href="../../properties/irepframelineint-color/">Color</a> | <a href="../../properties/irepframelineint-framestyle/">FrameStyle</a> | <a href="../../properties/irepframelineint-linebottom/">LineBottom</a> | <a href="../../properties/irepframelineint-lineleft/">LineLeft</a> | <a href="../../properties/irepframelineint-lineright/">LineRight</a> | <a href="../../properties/irepframelineint-linetop/">LineTop</a> | <a href="../../properties/irepframelineint-linetype/">LineType</a> | <a href="../../properties/irepframelineint-useindividuallinestyle/">UseIndividualLineStyle</a> | <a href="../../properties/irepframelineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcircleint/">Circle</a>.<a href="../../properties/irepcircleint-borderline/">BorderLine</a> | <a href="../irepcommenttextint/">CommentElement</a>.<a href="../../properties/irepcommenttextint-borderline/">BorderLine</a> | <a href="../irepfreeframeint/">Frame</a>.<a href="../../properties/irepfreeframeint-borderline/">BorderLine</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepFrameLineInt.htm`*
