---
title: "IRepImageInt.FileName"
description: "Specifies the path and the name of a graphic file in DIAdem REPORT. If you do not specify a path, DIAdem first searches for the graphic file in the user folder "
---

# IRepImageInt.FileName

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FileName for Image

Specifies the path and the name of a graphic file in DIAdem REPORT. If you do not specify a path, DIAdem first searches for the graphic file in the user folder and then in the library folder.

## Signature

```python
obj.FileName
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyPos = oMyImage.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.BackgroundColor.SetPredefinedColor(dd.eColorIndexNone)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FileName_IRepImageInt.htm`*
