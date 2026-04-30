---
title: "IRepFontInt.Color"
description: "Specifies the font color in DIAdem REPORT. DIAdem only includes the property Color in the 3DIsolineLabel2DAdditionalLabel , 3DIsolineLabel , AdditionalLineEndLa"
---

# IRepFontInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for Font

Specifies the font color in DIAdem REPORT. DIAdem only includes the property Color in the 3DIsolineLabel2DAdditionalLabel , 3DIsolineLabel , AdditionalLineEndLabel , AxisLabel , CurveLegendSettings , LabelNumeric and PolarSectorNumbers objects if you assign the value FALSE to the UseCurveColor property.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyFont = oMyComment.Comment.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 7
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepFontInt.htm`*
