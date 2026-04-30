---
title: "IRepPositionXYInt.Angle"
description: "Specifies the position of text in DIAdem REPORT as the angle between the text base and the bottom of the page."
---

# IRepPositionXYInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for ObjectPositionXY

Specifies the position of text in DIAdem REPORT as the angle between the text base and the bottom of the page.

## Signature

```python
obj.Angle
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a Text"
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

*Source: `ReportApi/properties/Report_property_Angle_IRepPositionXYInt.htm`*
