---
title: "IRepBackgroundColorInt.SetRGBColor"
description: "Assigns a background color to an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display a color."
---

# IRepBackgroundColorInt.SetRGBColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetRGBColor for BackgroundColor

Assigns a background color to an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display a color.

## Signature

```python
obj.SetRGBColor(RGB)
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.BackColor.SetRGBColor(dd.Rgb(255,0,0))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetRGBColor_IRepBackgroundColorInt.htm`*
