---
title: "IRepCtrlListInt.Add"
description: "Adds a new object to a worksheet in DIAdem REPORT."
---

# IRepCtrlListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for ReportObjects

Adds a new object to a worksheet in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(objType, Name)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eReportObject2DAxisSystem` | 0 | 2D axis system |
| `eReportObject2DTable` | 1 | 2D table |
| `eReportObjectPolarSystem` | 2 | Polar axis system |
| `eReportObject3DAxisSystem` | 3 | 3D axis system |
| `eReportObject3DTable` | 4 | 3D table |
| `eReportObjectText` | 5 | Text |
| `eReportObjectFrame` | 6 | Frame |
| `eReportObjectImage` | 7 | Graphic |
| `eReportObjectRTFText` | 8 | Text object |
| `eReportObjectArrow` | 9 | Line and arrow |
| `eReportObjectComment` | 10 | Comment |
| `eReportObjectCircle` | 11 | Circle |
| `eReportObjectFormulaDisplay` | 12 | Formula graphic |
| `eReportObjectSpider` | 13 | Spider axis system |
| `eReportObjectPieChart` | 14 | Pie chart |

## Python example

```python
if dd.Report.ActiveSheet.Objects.Exists("MyCircle") :
    dd.MsgBoxDisp("Object \"MyCircle\" already exists.")
else:
    oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
    oMyCircle.Position.ByBorder.Left = 30
    oMyCircle.Position.ByBorder.Bottom = 30
    oMyCircle.Position.ByBorder.Height = 40
    oMyCircle.Position.ByBorder.Width = 40
    oMyCircle.BackgroundColor.SetPredefinedColor(dd.eColorIndexBlue)
    oMyCircle.BorderLine.Color.SetPredefinedColor(dd.eColorIndexRed)
    dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepCtrlListInt.htm`*
