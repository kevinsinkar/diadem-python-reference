---
title: "IRepSettingsImageExportJPGInt"
description: "The SettingsImageExportJPG object provides the export properties of a layout in a JPG file."
---

# IRepSettingsImageExportJPGInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SettingsImageExportJPG

The SettingsImageExportJPG object provides the export properties of a layout in a JPG file.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyJPGExport = dd.Report.Settings.ImageExport.JPG
oMyJPGExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyJPGExport.Height = 300
oMyJPGExport.UseRatio = True
oMyJPGExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeJPG)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsimageexportjpgint-bitsperpixel/">BitsPerPixel</a> | <a href="../../properties/irepsettingsimageexportjpgint-compression/">Compression</a> | <a href="../../properties/irepsettingsimageexportjpgint-height/">Height</a> | <a href="../../properties/irepsettingsimageexportjpgint-progressive/">Progressive</a> | <a href="../../properties/irepsettingsimageexportjpgint-useratio/">UseRatio</a> | <a href="../../properties/irepsettingsimageexportjpgint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsimageexportint/">SettingsImageExport</a>.<a href="../../properties/irepsettingsimageexportint-jpg/">JPG</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsImageExportJPGInt.htm`*
