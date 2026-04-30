---
title: "IRepSettingsInt"
description: "The Settings object provides the general settings in DIAdem REPORT."
---

# IRepSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Settings

The Settings object provides the general settings in DIAdem REPORT.

## Python example

```python
oMyCurveExpandObj = dd.Report.Settings.CurveExpansion
oMyExpandLine = oMyCurveExpandObj.AttributeList.LineStyles
oMyCurveExpandObj.Enable = True
oMyCurveExpandObj.AttributeList.Enable = True
for I in range( 1, oMyExpandLine.Count+1):
    oMyExpandLine.Item(I).Line.Width = dd.eLineWidth0070
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsint-channeltransformationconfiguration/">ChannelTransformationConfiguration</a> | <a href="../../properties/irepsettingsint-curve2dtransformationconfiguration/">Curve2DTransformationConfiguration</a> | <a href="../../properties/irepsettingsint-curve3dtransformationconfiguration/">Curve3DTransformationConfiguration</a> | <a href="../../properties/irepsettingsint-curveexpansion/">CurveExpansion</a> | <a href="../../properties/irepsettingsint-customscaling/">CustomScaling</a> | <a href="../../properties/irepsettingsint-defaultfontname/">DefaultFontName</a> | <a href="../../properties/irepsettingsint-defaultfonttype/">DefaultFontType</a> | <a href="../../properties/irepsettingsint-export/">Export</a> | <a href="../../properties/irepsettingsint-globalcolorpalette1/">GlobalColorPalette1</a> | <a href="../../properties/irepsettingsint-globalcolorpalette2/">GlobalColorPalette2</a> | <a href="../../properties/irepsettingsint-globalcolorpalette3/">GlobalColorPalette3</a> | <a href="../../properties/irepsettingsint-imageexport/">ImageExport</a> | <a href="../../properties/irepsettingsint-masterlayout/">MasterLayout</a> | <a href="../../properties/irepsettingsint-page/">Page</a> | <a href="../../properties/irepsettingsint-synchronization/">Synchronization</a> | <a href="../../properties/irepsettingsint-useautoscalingnormseries/">UseAutoScalingNormSeries</a> | <a href="../../properties/irepsettingsint-usetransparencywhileprinting/">UseTransparencyWhilePrinting</a> | <a href="../../properties/irepsettingsint-usevirtualprintmemory/">UseVirtualPrintMemory</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepsettingsint-converttochannelreferencebyname/">ConvertToChannelReferenceByName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepreportint/">Report</a>.<a href="../../properties/irepreportint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsInt.htm`*
