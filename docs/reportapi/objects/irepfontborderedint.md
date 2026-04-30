---
title: "IRepFontBorderedInt"
description: "The FontWithBorder object provides font properties in DIAdem REPORT."
---

# IRepFontBorderedInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: FontWithBorder

The FontWithBorder object provides font properties in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a text"
oMyFont = oMyText.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 10
oMyFont.Border = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepfontborderedint-backcolor/">BackColor</a> | <a href="../../properties/irepfontborderedint-bold/">Bold</a> | <a href="../../properties/irepfontborderedint-border/">Border</a> | <a href="../../properties/irepfontborderedint-color/">Color</a> | <a href="../../properties/irepfontborderedint-italic/">Italic</a> | <a href="../../properties/irepfontborderedint-name/">Name</a> | <a href="../../properties/irepfontborderedint-size/">Size</a> | <a href="../../properties/irepfontborderedint-strikeout/">StrikeOut</a> | <a href="../../properties/irepfontborderedint-underline/">Underline</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2labeladditionalint/">2DAdditionalLabel</a>.<a href="../../properties/irepd2labeladditionalint-font/">Font</a> | <a href="../ireptable2dcolheaderfooterindisettingsint/">2DTableColumnHeaderFooterIndividualSettings</a>.<a href="../../properties/ireptable2dcolheaderfooterindisettingsint-font/">Font</a> | <a href="../ireptable2dcolumnsettingsint/">2DTableColumnSettings</a>.<a href="../../properties/ireptable2dcolumnsettingsint-font/">Font</a> | <a href="../ireptable2ddrawingcellint/">2DTableDrawingCell</a>.<a href="../../properties/ireptable2ddrawingcellint-font/">Font</a> | <a href="../ireptable2ddrawingheaderfootercellint/">2DTableDrawingHeaderFooterCell</a>.<a href="../../properties/ireptable2ddrawingheaderfootercellint-font/">Font</a> | <a href="../ireptable2dheaderdefaultsettingsint/">2DTableHeaderFooterDefaultSettings</a>.<a href="../../properties/ireptable2dheaderdefaultsettingsint-font/">Font</a> | <a href="../irepd3labelisolineadditionalint/">3DAdditionalIsolineLabel</a>.<a href="../../properties/irepd3labelisolineadditionalint-font/">Font</a> | <a href="../irepd3labeladditionalint/">3DAdditionalLabel</a>.<a href="../../properties/irepd3labeladditionalint-font/">Font</a> | <a href="../irepd3characteristicdiagrampointslabelint/">3DCharacteristicDiagramPointsLabel</a>.<a href="../../properties/irepd3characteristicdiagrampointslabelint-font/">Font</a> | <a href="../irepd3isolinelabelint/">3DIsolineLabel</a>.<a href="../../properties/irepd3isolinelabelint-font/">Font</a> | <a href="../irepconstantlabeladditionalint/">AdditionalConstantLabel</a>.<a href="../../properties/irepconstantlabeladditionalint-font/">Font</a> | <a href="../irepcoordinatelabeladditionalint/">AdditionalCoordinateLabel</a>.<a href="../../properties/irepcoordinatelabeladditionalint-font/">Font</a> | <a href="../ireplineendlabeladditionalint/">AdditionalLineEndLabel</a>.<a href="../../properties/ireplineendlabeladditionalint-font/">Font</a> | <a href="../irepaxislabelint/">AxisLabel</a>.<a href="../../properties/irepaxislabelint-font/">Font</a> | <a href="../ireplabelnumericint/">LabelNumeric</a>.<a href="../../properties/ireplabelnumericint-font/">Font</a> | <a href="../ireplabelnumericyint/">LabelNumericY</a>.<a href="../../properties/ireplabelnumericyint-font/">Font</a> | <a href="../ireppiechartslicelabelint/">PieChartSliceLabel</a>.<a href="../../properties/ireppiechartslicelabelint-font/">Font</a> | <a href="../ireppolarlabeladditionalint/">PolarAdditionalLabel</a>.<a href="../../properties/ireppolarlabeladditionalint-font/">Font</a> | <a href="../ireppolarpointsint/">PolarPoints</a>.<a href="../../properties/ireppolarpointsint-font/">Font</a> | <a href="../ireppolarsectorlabelnumericint/">PolarSectorNumbers</a>.<a href="../../properties/ireppolarsectorlabelnumericint-font/">Font</a> | <a href="../irepspiderlabeladditionalint/">SpiderAdditionalLabel</a>.<a href="../../properties/irepspiderlabeladditionalint-font/">Font</a> | <a href="../irepspiderlabelnumericint/">SpiderLabelNumeric</a>.<a href="../../properties/irepspiderlabelnumericint-font/">Font</a> | <a href="../ireptextsimpleint/">Text</a>.<a href="../../properties/ireptextsimpleint-font/">Font</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepFontBorderedInt.htm`*
