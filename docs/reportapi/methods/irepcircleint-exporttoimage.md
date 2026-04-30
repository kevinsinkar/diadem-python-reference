---
title: "IRepCircleInt.ExportToImage"
description: "Exports a circle from DIAdem REPORT to a graphics file."
---

# IRepCircleInt.ExportToImage

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ExportToImage for Circle

Exports a circle from DIAdem REPORT to a graphics file.

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
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")

oMyCircle.ForceCircle = True

oMyBackgroundColor = oMyCircle.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyBackgroundColor.Transparency = 50

oMyCircle.Position.ByCoordinate.X1 = 10
oMyCircle.Position.ByCoordinate.X2 = 40
oMyCircle.Position.ByCoordinate.Y1 = 50
oMyCircle.Position.ByCoordinate.Y2 = 80

oMyBorderLineColor = oMyCircle.BorderLine.Color
oMyBorderLineColor.SetPredefinedColor(dd.eColorIndexGreen)
oMyCircle.BorderLine.LineType = dd.eLineTypeDotted
oMyCircle.BorderLine.Width = dd.eLineWidth0140

dd.Report.Settings.ImageExport.PNG.BitsPerPixel = dd.ePNGBitsPerPixelRGB24
dd.Report.Settings.ImageExport.PNG.Height = 300
dd.Report.Settings.ImageExport.PNG.UseRatio = True
oMyCircle.ExportToImage(dd.LayoutWritePath + "MyCircle", dd.eImageExportTypePNG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ExportToImage_IRepCircleInt.htm`*
