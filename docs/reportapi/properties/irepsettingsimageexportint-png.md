---
title: "IRepSettingsImageExportInt.PNG"
description: "Specifies the properties for the export of a REPORT layout into a PNG file."
---

# IRepSettingsImageExportInt.PNG

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PNG for SettingsImageExport

Specifies the properties for the export of a REPORT layout into a PNG file.

## Signature

```python
return_value = obj.PNG
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PNG_IRepSettingsImageExportInt.htm`*
