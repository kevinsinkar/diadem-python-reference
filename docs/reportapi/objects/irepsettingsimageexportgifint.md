---
title: "IRepSettingsImageExportGIFInt"
description: "The SettingsImageExportGIF object provides the export properties of a layout in a GIF file."
---

# IRepSettingsImageExportGIFInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SettingsImageExportGIF

The SettingsImageExportGIF object provides the export properties of a layout in a GIF file.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Settings.ImageExport.GIF.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
dd.Report.Settings.ImageExport.GIF.Height = 300
dd.Report.Settings.ImageExport.GIF.UseRatio = True
dd.Report.Settings.ImageExport.GIF.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyNew2DCurve", dd.eImageExportTypeGIF)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsimageexportgifint-bitsperpixel/">BitsPerPixel</a> | <a href="../../properties/irepsettingsimageexportgifint-height/">Height</a> | <a href="../../properties/irepsettingsimageexportgifint-useratio/">UseRatio</a> | <a href="../../properties/irepsettingsimageexportgifint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsimageexportint/">SettingsImageExport</a>.<a href="../../properties/irepsettingsimageexportint-gif/">GIF</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsImageExportGIFInt.htm`*
