---
title: "IRepBackgroundColorInt"
description: "The BackgroundColor object provides the background color of an object in DIAdem REPORT."
---

# IRepBackgroundColorInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: BackgroundColor

The BackgroundColor object provides the background color of an object in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.BackColor.SetPredefinedColor(dd.ePredefinedColorDarkRed)
```

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.BackColor.SetFillingColor(dd.Rgb(255,0,9), dd.Rgb(0,255,0), dd.eColorGradientHorizontal, dd.eColorGradientModeFromBottom)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepbackgroundcolorint-colorindex/">ColorIndex</a> | <a href="../../properties/irepbackgroundcolorint-gradientdirection/">GradientDirection</a> | <a href="../../properties/irepbackgroundcolorint-gradientmode/">GradientMode</a> | <a href="../../properties/irepbackgroundcolorint-rgb/">RGB</a> | <a href="../../properties/irepbackgroundcolorint-rgbfilling/">RGBFilling</a> | <a href="../../properties/irepbackgroundcolorint-transparency/">Transparency</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepbackgroundcolorint-setfillingcolor/">SetFillingColor</a> | <a href="../../methods/irepbackgroundcolorint-setpredefinedcolor/">SetPredefinedColor</a> | <a href="../../methods/irepbackgroundcolorint-setrgbcolor/">SetRGBColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axissettingsint/">2DAxisSettings</a>.<a href="../../properties/irepd2axissettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2dcolheaderfooterindisettingsint/">2DTableColumnHeaderFooterIndividualSettings</a>.<a href="../../properties/ireptable2dcolheaderfooterindisettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2dcolumnsettingsint/">2DTableColumnSettings</a>.<a href="../../properties/ireptable2dcolumnsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2ddrawingcellint/">2DTableDrawingCell</a>.<a href="../../properties/ireptable2ddrawingcellint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2ddrawingheaderfootercellint/">2DTableDrawingHeaderFooterCell</a>.<a href="../../properties/ireptable2ddrawingheaderfootercellint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2dheaderdefaultsettingsint/">2DTableHeaderFooterDefaultSettings</a>.<a href="../../properties/ireptable2dheaderdefaultsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2dbackgroundcolors/">2DTableItemBackgroundColor</a>.<a href="../../properties/ireptable2dbackgroundcolors-alternatingbackgroundcolor/">AlternatingBackgroundColor</a> | <a href="../ireptable2dbackgroundcolors/">2DTableItemBackgroundColor</a>.<a href="../../properties/ireptable2dbackgroundcolors-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../irepd3planexyint/">3DPlaneXY</a>.<a href="../../properties/irepd3planexyint-backgroundcolor/">BackgroundColor</a> | <a href="../irepd3planexzint/">3DPlaneXZ</a>.<a href="../../properties/irepd3planexzint-backgroundcolor/">BackgroundColor</a> | <a href="../irepd3planeyzint/">3DPlaneYZ</a>.<a href="../../properties/irepd3planeyzint-backgroundcolor/">BackgroundColor</a> | <a href="../ireptable3dsettingsint/">3DTableSettings</a>.<a href="../../properties/ireptable3dsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcommenttextadditionalint/">AdditionalCommentText</a>.<a href="../../properties/irepcommenttextadditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../irepconstantlabeladditionalint/">AdditionalConstantLabel</a>.<a href="../../properties/irepconstantlabeladditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcoordinatelabeladditionalint/">AdditionalCoordinateLabel</a>.<a href="../../properties/irepcoordinatelabeladditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../ireplineendlabeladditionalint/">AdditionalLineEndLabel</a>.<a href="../../properties/ireplineendlabeladditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcircleint/">Circle</a>.<a href="../../properties/irepcircleint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcolorlegendsettingsint/">ColorLegendSettings</a>.<a href="../../properties/irepcolorlegendsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcommenttextint/">CommentElement</a>.<a href="../../properties/irepcommenttextint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcurvelegendsettingsint/">CurveLegendSettings</a>.<a href="../../properties/irepcurvelegendsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../irepfontint/">Font</a>.<a href="../../properties/irepfontint-backcolor/">BackColor</a> | <a href="../irepfontborderedint/">FontWithBorder</a>.<a href="../../properties/irepfontborderedint-backcolor/">BackColor</a> | <a href="../irepfreeframeint/">Frame</a>.<a href="../../properties/irepfreeframeint-backgroundcolor/">BackgroundColor</a> | <a href="../irepcomformulasubframeint/">FrameElement</a>.<a href="../../properties/irepcomformulasubframeint-backgroundcolor/">BackgroundColor</a> | <a href="../irepimageint/">Image</a>.<a href="../../properties/irepimageint-backgroundcolor/">BackgroundColor</a> | <a href="../ireppagedefaultsettingsint/">PageDefaultSettings</a>.<a href="../../properties/ireppagedefaultsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../ireppolarsettingsint/">PolarSettings</a>.<a href="../../properties/ireppolarsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../irepspidersettingsint/">SpiderSettings</a>.<a href="../../properties/irepspidersettingsint-backgroundcolor/">BackgroundColor</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepBackgroundColorInt.htm`*
