---
title: "IRepFontInt"
description: "The Font object provides font properties in DIAdem REPORT."
---

# IRepFontInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Font

The Font object provides font properties in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyFont = oMyComment.Comment.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 7
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepfontint-backcolor/">BackColor</a> | <a href="../../properties/irepfontint-bold/">Bold</a> | <a href="../../properties/irepfontint-color/">Color</a> | <a href="../../properties/irepfontint-italic/">Italic</a> | <a href="../../properties/irepfontint-name/">Name</a> | <a href="../../properties/irepfontint-size/">Size</a> | <a href="../../properties/irepfontint-strikeout/">StrikeOut</a> | <a href="../../properties/irepfontint-underline/">Underline</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3characteristicdiagramhyperbolaadditionalint/">3DAdditionalHyperbolaLines</a>.<a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-font/">Font</a> | <a href="../ireptable3dheaderint/">3DTableHeader</a>.<a href="../../properties/ireptable3dheaderint-font/">Font</a> | <a href="../ireptable3dxvaluesint/">3DTableXValues</a>.<a href="../../properties/ireptable3dxvaluesint-font/">Font</a> | <a href="../ireptable3dyvaluesint/">3DTableYValues</a>.<a href="../../properties/ireptable3dyvaluesint-font/">Font</a> | <a href="../ireptable3dzvaluesint/">3DTableZValues</a>.<a href="../../properties/ireptable3dzvaluesint-font/">Font</a> | <a href="../irepcommenttextadditionalint/">AdditionalCommentText</a>.<a href="../../properties/irepcommenttextadditionalint-font/">Font</a> | <a href="../irepcolorlegendheaderint/">ColorLegendHeader</a>.<a href="../../properties/irepcolorlegendheaderint-font/">Font</a> | <a href="../irepcolorlegendsettingsint/">ColorLegendSettings</a>.<a href="../../properties/irepcolorlegendsettingsint-font/">Font</a> | <a href="../irepcommenttextint/">CommentElement</a>.<a href="../../properties/irepcommenttextint-font/">Font</a> | <a href="../irepcurvelegendheaderint/">CurveLegendHeader</a>.<a href="../../properties/irepcurvelegendheaderint-font/">Font</a> | <a href="../irepcurvelegendsettingsint/">CurveLegendSettings</a>.<a href="../../properties/irepcurvelegendsettingsint-font/">Font</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepFontInt.htm`*
