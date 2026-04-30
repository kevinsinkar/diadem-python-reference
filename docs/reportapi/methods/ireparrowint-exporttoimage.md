---
title: "IRepArrowInt.ExportToImage"
description: "Exports an arrow from DIAdem REPORT to a graphics file."
---

# IRepArrowInt.ExportToImage

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ExportToImage for Arrow

Exports an arrow from DIAdem REPORT to a graphics file.

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
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow,"MyArrow")

oMyArrow.ArrowHeadAtBegin = dd.eArrowHeadPoint
oMyArrow.ArrowHeadAtEnd = dd.eArrowHeadStandardArrow

oMyArrowPosition = oMyArrow.Position.ByCoordinate
oMyArrowPosition.X1 = 10
oMyArrowPosition.X2 = 40
oMyArrowPosition.Y1 = 30
oMyArrowPosition.Y2 = 90

oMyArrowLine = oMyArrow.Line
oMyArrowLine.LineType = dd.eLineTypeDotted
oMyArrowLine.Width = dd.eLineWidth0200

oMyArrowLineColor = oMyArrowLine.Color
oMyArrowLineColor.SetPredefinedColor(dd.eColorIndexGreen)

dd.Report.Settings.ImageExport.PNG.BitsPerPixel = dd.ePNGBitsPerPixelRGB24
dd.Report.Settings.ImageExport.PNG.Height = 300
dd.Report.Settings.ImageExport.PNG.UseRatio = True
oMyArrow.ExportToImage(dd.LayoutWritePath + "MyNewArrow", dd.eImageExportTypePNG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ExportToImage_IRepArrowInt.htm`*
