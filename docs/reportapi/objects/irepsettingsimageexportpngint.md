---
title: "IRepSettingsImageExportPNGInt"
description: "The SettingsImageExportPNG object provides the export properties of a layout in a PNG file."
---

# IRepSettingsImageExportPNGInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SettingsImageExportPNG

The SettingsImageExportPNG object provides the export properties of a layout in a PNG file.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyPNGExport = dd.Report.Settings.ImageExport.PNG
oMyPNGExport.BitsPerPixel = dd.ePNGBitsPerPixelRGB32
oMyPNGExport.Height = 300
oMyPNGExport.UseRatio = True
oMyPNGExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypePNG)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsimageexportpngint-bitsperpixel/">BitsPerPixel</a> | <a href="../../properties/irepsettingsimageexportpngint-height/">Height</a> | <a href="../../properties/irepsettingsimageexportpngint-useratio/">UseRatio</a> | <a href="../../properties/irepsettingsimageexportpngint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsimageexportint/">SettingsImageExport</a>.<a href="../../properties/irepsettingsimageexportint-png/">PNG</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsImageExportPNGInt.htm`*
