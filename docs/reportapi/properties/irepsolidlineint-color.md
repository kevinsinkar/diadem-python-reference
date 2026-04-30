---
title: "IRepSolidLineInt.Color"
description: "Specifies the color of a line in DIAdem REPORT. DIAdem only includes the Color property in the 2DAxisSettings object if you assign the value TRUE to the UseIndi"
---

# IRepSolidLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for SolidLine

Specifies the color of a line in DIAdem REPORT. DIAdem only includes the Color property in the 2DAxisSettings object if you assign the value TRUE to the UseIndividualAxisStyle property.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Report.NewLayout()
oMyBorderLine = dd.Report.Settings.Page.BorderLine
oMyBorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyBorderLine.Width = dd.eLineWidth1120
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepSolidLineInt.htm`*
