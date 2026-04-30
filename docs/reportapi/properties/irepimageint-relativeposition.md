---
title: "IRepImageInt.RelativePosition"
description: "Specifies the position of a graphic relative to the specified position in DIAdem REPORT."
---

# IRepImageInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for Image

Specifies the position of a graphic relative to the specified position in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionPointRightTop` | 0 | Top right |
| `eRelativePositionPointCenter` | 1 | Centered |
| `eRelativePositionPointRight` | 2 | Right |
| `eRelativePositionPointRightBottom` | 3 | Bottom right |
| `eRelativePositionPointTop` | 4 | Top |
| `eRelativePositionPointBottom` | 5 | Bottom |
| `eRelativePositionPointLeftTop` | 6 | Top left |
| `eRelativePositionPointLeft` | 7 | Left |
| `eRelativePositionPointLeftBottom` | 8 | Bottom left |

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
oMyImage.RelativePosition = dd.eRelativePositionLeftBottom
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepImageInt.htm`*
