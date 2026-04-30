---
title: "IRepPositionXYInt.Y"
description: "Specifies the margin between the text and the bottom of a DIAdem REPORT page as a percentage of the worksheet, in centimeters or inches. The text position is sp"
---

# IRepPositionXYInt.Y

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Y for ObjectPositionXY

Specifies the margin between the text and the bottom of a DIAdem REPORT page as a percentage of the worksheet, in centimeters or inches. The text position is specified in relation to the text anchor point.

## Signature

```python
obj.Y
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a text"
oMyPosition = oMyText.PositionXY
oMyPosition.RelativePosition = dd.eRelativePositionRightTop
oMyPosition.X = 10
oMyPosition.Y = 20
oMyPosition.Angle = 45
oMyFont = oMyText.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 10
oMyFont.Border = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Y_IRepPositionXYInt.htm`*
