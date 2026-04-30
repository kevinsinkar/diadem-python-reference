---
title: "IRepImageInt.UseOriginalRatio"
description: "Specifies whether DIAdem REPORT maintains the height-to-width ratio of a graphic."
---

# IRepImageInt.UseOriginalRatio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseOriginalRatio for Image

Specifies whether DIAdem REPORT maintains the height-to-width ratio of a graphic.

## Signature

```python
obj.UseOriginalRatio
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.UseOriginalRatio = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseOriginalRatio_IRepImageInt.htm`*
