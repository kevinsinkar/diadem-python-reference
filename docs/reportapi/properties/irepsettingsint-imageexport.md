---
title: "IRepSettingsInt.ImageExport"
description: "Specifies in DIAdem REPORT the properties for the export of a layout in a graphic file. You can export layouts in JPG, GIF, TIF, and PNG files."
---

# IRepSettingsInt.ImageExport

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ImageExport for Settings

Specifies in DIAdem REPORT the properties for the export of a layout in a graphic file. You can export layouts in JPG, GIF, TIF, and PNG files.

## Signature

```python
return_value = obj.ImageExport
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
OMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
OMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Settings.ImageExport.GIF.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
dd.Report.Settings.ImageExport.GIF.Height = 300
dd.Report.Settings.ImageExport.GIF.UseRatio = True
dd.Report.Settings.ImageExport.GIF.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyNew2DCurve", dd.eImageExportTypeGIF)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ImageExport_IRepSettingsInt.htm`*
