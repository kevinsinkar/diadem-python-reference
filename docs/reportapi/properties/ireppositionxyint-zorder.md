---
title: "IRepPositionXYInt.ZOrder"
description: "Specifies the order of a text in DIAdem REPORT."
---

# IRepPositionXYInt.ZOrder

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ZOrder for ObjectPositionXY

Specifies the order of a text in DIAdem REPORT.

## Signature

```python
return_value = obj.ZOrder
```

## Python example

```python
dd.Report.NewLayout()
oMyText1 = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText1")
oMyText1.Text = "This is the first text"
oMyPosition1 = oMyText1.PositionXY
oMyPosition1.X = 30
oMyPosition1.Y = 40
oMyPosition1.Angle = 25
oMyText1.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyText1.Font.Name = "Tahoma"
oMyText1.Font.Size = 10
oMyText1.Font.Border = True
oMyText2 = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText2")
oMyText2.Text = "This is the second text"
oMyPosition2 = oMyText2.PositionXY
oMyPosition2.X = 50
oMyPosition2.Y = 60
oMyPosition2.Angle = 75
oMyText2.Font.Name = "Times Roman"()
oMyText2.Font.Size = 11
oMyText2.Font.Border = False
dd.MsgBoxDisp("Layer:" + oMyPosition2.ZOrder.Order)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ZOrder_IRepPositionXYInt.htm`*
