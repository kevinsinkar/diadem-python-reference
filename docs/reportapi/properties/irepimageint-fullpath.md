---
title: "IRepImageInt.FullPath"
description: "Specifies the complete path and the filename of a graphics file in DIAdem REPORT."
---

# IRepImageInt.FullPath

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FullPath for Image

Specifies the complete path and the filename of a graphics file in DIAdem REPORT.

## Signature

```python
obj.FullPath
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.BackgroundColor.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.MsgBoxDisp(oMyImage.Fullpath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FullPath_IRepImageInt.htm`*
