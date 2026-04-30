---
title: "IRepSettingsImageExportInt.GIF"
description: "Specifies the properties for the export of a layout in a GIF file."
---

# IRepSettingsImageExportInt.GIF

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GIF for SettingsImageExport

Specifies the properties for the export of a layout in a GIF file.

## Signature

```python
return_value = obj.GIF
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

*Source: `ReportApi/properties/Report_property_GIF_IRepSettingsImageExportInt.htm`*
