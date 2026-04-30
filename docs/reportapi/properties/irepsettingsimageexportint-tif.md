---
title: "IRepSettingsImageExportInt.TIF"
description: "Specifies the properties for the export of a layout in a TIF file."
---

# IRepSettingsImageExportInt.TIF

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TIF for SettingsImageExport

Specifies the properties for the export of a layout in a TIF file.

## Signature

```python
return_value = obj.TIF
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TIF_IRepSettingsImageExportInt.htm`*
