---
title: "IRepTextSimpleInt.PositionXY"
description: "Specifies the position of a text in a DIAdem REPORT worksheet."
---

# IRepTextSimpleInt.PositionXY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PositionXY for Text

Specifies the position of a text in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.PositionXY
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PositionXY_IRepTextSimpleInt.htm`*
