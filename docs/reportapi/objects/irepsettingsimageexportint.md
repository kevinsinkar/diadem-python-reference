---
title: "IRepSettingsImageExportInt"
description: "The SettingsImageExport object provides the export properties of a layout in a graphics file."
---

# IRepSettingsImageExportInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SettingsImageExport

The SettingsImageExport object provides the export properties of a layout in a graphics file.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyGIFExport = dd.Report.Settings.ImageExport.GIF
oMyGIFExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyGIFExport.Height = 300
oMyGIFExport.UseRatio = True
oMyGIFExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeGIF)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsimageexportint-gif/">GIF</a> | <a href="../../properties/irepsettingsimageexportint-jpg/">JPG</a> | <a href="../../properties/irepsettingsimageexportint-png/">PNG</a> | <a href="../../properties/irepsettingsimageexportint-tif/">TIF</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-imageexport/">ImageExport</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsImageExportInt.htm`*
