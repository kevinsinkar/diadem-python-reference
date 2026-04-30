---
title: "IRepPositionXYInt.RelativePosition"
description: "Specifies the anchor point for text in DIAdem REPORT."
---

# IRepPositionXYInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for ObjectPositionXY

Specifies the anchor point for text in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionRightTop` | 0 | Top right |
| `eRelativePositionCenter` | 1 | Center |
| `eRelativePositionRight` | 2 | Right |
| `eRelativePositionRightBottom` | 3 | Bottom right |
| `eRelativePositionTop` | 4 | Top |
| `eRelativePositionBottom` | 5 | Bottom |
| `eRelativePositionLeftTop` | 6 | Top left |
| `eRelativePositionLeft` | 7 | Left |
| `eRelativePositionLeftBottom` | 8 | Bottom left |

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a Text"
oMyPosition = oMyText.PositionXY
oMyPosition.RelativePosition = dd.eRelativePositionRightTop
oMyPosition.X = 10
oMyPosition.Y = 20
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

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepPositionXYInt.htm`*
