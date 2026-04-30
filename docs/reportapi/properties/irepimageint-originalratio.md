---
title: "IRepImageInt.OriginalRatio"
description: "Specifies the height/width ratio of a graphic in DIAdem REPORT in relation to the height/width ratio of the worksheet that contains the graphic. If, for example"
---

# IRepImageInt.OriginalRatio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OriginalRatio for Image

Specifies the height/width ratio of a graphic in DIAdem REPORT in relation to the height/width ratio of the worksheet that contains the graphic. If, for example, you display a square graphic with a size of 10*10 on a worksheet with a page ratio of 0.7 , the OriginalRatio property also has the value 0.7.

## Signature

```python
obj.OriginalRatio
```

## Python example

```python
oMySheet = dd.Report.Sheets.Add("NewSheet")
oMyReportObj = oMySheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyReportObj.FileName = dd.LayoutLibrPath + "EXAMPLE3.GIF"
oMyReportObj.Position.ByBorder.Bottom = 40
oMyReportObj.Position.ByBorder.Left = 40
oMyReportObj.Position.ByBorder.Height = 20
oMyReportObj.Position.ByBorder.Width = 20
dd.MsgBoxDisp("Ratio: " + oMyReportObj.OriginalRatio)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OriginalRatio_IRepImageInt.htm`*
