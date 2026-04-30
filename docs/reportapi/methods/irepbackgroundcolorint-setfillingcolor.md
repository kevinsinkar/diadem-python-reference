---
title: "IRepBackgroundColorInt.SetFillingColor"
description: "Specifies the filling effects of the highlighting color of an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary"
---

# IRepBackgroundColorInt.SetFillingColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetFillingColor for BackgroundColor

Specifies the filling effects of the highlighting color of an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display the filling effects. Not all REPORT objects display filling effects.

## Signature

```python
obj.SetFillingColor(RGB1, RGB2, GradientDirection, GradientMode)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorGradientHorizontal` | 0 | Horizontal |
| `eColorGradientVertical` | 1 | Vertical |
| `eColorGradientDiagonalLeft` | 2 | Diagonal left |
| `eColorGradientDiagonalRight` | 3 | Diagonal right |
| `eColorGradientModeFromBottom` | 0 | Up |
| `eColorGradientModeFromTop` | 1 | Down |
| `eColorGradientModeFromInside` | 2 | From inside |
| `eColorGradientModeFromOutside` | 3 | From outside |
| `eColorGradientModeSectors` | 5 | Section wise |

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.BackColor.SetFillingColor(dd.Rgb(255,0,9), dd.Rgb(0,255,0), dd.eColorGradientHorizontal, dd.eColorGradientModeFromBottom)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetFillingColor_IRepBackgroundColorInt.htm`*
