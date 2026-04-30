---
title: "IRepPositionXYInt.X"
description: "Specifies the distance between the text and the left edge of a page, in centimeters or inches, as a percentage of the worksheet in DIAdem REPORT. The text posit"
---

# IRepPositionXYInt.X

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: X for ObjectPositionXY

Specifies the distance between the text and the left edge of a page, in centimeters or inches, as a percentage of the worksheet in DIAdem REPORT. The text position is specified in relation to the text anchor point.

## Signature

```python
obj.X
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

*Source: `ReportApi/properties/Report_property_X_IRepPositionXYInt.htm`*
