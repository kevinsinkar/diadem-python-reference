---
title: "IRepSettingsImageExportTIFInt"
description: "The SettingsImageExportTIF object provides the properties for exporting a layout to a TIF file."
---

# IRepSettingsImageExportTIFInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SettingsImageExportTIF

The SettingsImageExportTIF object provides the properties for exporting a layout to a TIF file.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyTIFExport = dd.Report.Settings.ImageExport.TIF
oMyTIFExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyTIFExport.Height = 300
oMyTIFExport.UseCompression = False
oMyTIFExport.UseRatio = True
oMyTIFExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeTIF)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsimageexporttifint-bitsperpixel/">BitsPerPixel</a> | <a href="../../properties/irepsettingsimageexporttifint-height/">Height</a> | <a href="../../properties/irepsettingsimageexporttifint-usecompression/">UseCompression</a> | <a href="../../properties/irepsettingsimageexporttifint-useratio/">UseRatio</a> | <a href="../../properties/irepsettingsimageexporttifint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsimageexportint/">SettingsImageExport</a>.<a href="../../properties/irepsettingsimageexportint-tif/">TIF</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsImageExportTIFInt.htm`*
