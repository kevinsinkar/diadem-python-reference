---
title: "IRepSettingsImageExportJPGInt.Compression"
description: "Specifies in DIAdem REPORT the degree of compression of a layout exported in the JPG format. You can assign a value between 0 and 100 to the Compression propert"
---

# IRepSettingsImageExportJPGInt.Compression

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Compression for SettingsImageExportJPG

Specifies in DIAdem REPORT the degree of compression of a layout exported in the JPG format. You can assign a value between 0 and 100 to the Compression property. The higher the value, the smaller the file and the lower the quality.

## Signature

```python
obj.Compression
```

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
oMyJPGExport.Compression = 50
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeJPG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Compression_IRepSettingsImageExportJPGInt.htm`*
