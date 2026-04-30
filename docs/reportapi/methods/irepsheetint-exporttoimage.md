---
title: "IRepSheetInt.ExportToImage"
description: "Exports a worksheet from DIAdem REPORT to a graphics file."
---

# IRepSheetInt.ExportToImage

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ExportToImage for Sheet

Exports a worksheet from DIAdem REPORT to a graphics file.

## Signature

```python
obj.ExportToImage(FileName, ImageType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eImageExportTypeEMF` | 1 | EMF file |
| `eImageExportTypePNG` | 2 | PNG file |
| `eImageExportTypeJPG` | 3 | JPG file |
| `eImageExportTypeGIF` | 4 | GIF file |
| `eImageExportTypeTIF` | 5 | TIF file |

## Python example

```python
dd.Report.Settings.ImageExport.PNG.BitsPerPixel = dd.ePNGBitsPerPixelRGB08
dd.Report.Settings.ImageExport.PNG.Height = 300
dd.Report.Settings.ImageExport.PNG.UseRatio = True
i = 0
oMyReportObjects = dd.Report.Sheets
for oMyReportObj in oMyReportObjects:
    oMyReportObj.ExportToImage(dd.LayoutWritePath + "MyExportFile" + i, dd.eImageExportTypePNG)
    i = i+1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ExportToImage_IRepSheetInt.htm`*
