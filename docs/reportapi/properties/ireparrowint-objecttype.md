---
title: "IRepArrowInt.ObjectType"
description: "Specifies the object type in DIAdem REPORT."
---

# IRepArrowInt.ObjectType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ObjectType for Arrow

Specifies the object type in DIAdem REPORT.

## Signature

```python
obj.ObjectType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eReportObject2DAxisSystem` | 0 | 2D axis system |
| `eReportObject2DTable` | 1 | 2D Table |
| `eReportObjectPolarSystem` | 2 | 2D polar axis system |
| `eReportObject3DAxisSystem` | 3 | 3D axis system |
| `eReportObject3DTable` | 4 | 3D table |
| `eReportObjectText` | 5 | Free text |
| `eReportObjectFrame` | 6 | Rectangle |
| `eReportObjectImage` | 7 | Any graphic |
| `eReportObjectRTFText` | 8 | Text object |
| `eReportObjectArrow` | 9 | Line and arrow |
| `eReportObjectComment` | 10 | Comment |
| `eReportObjectCircle` | 11 | Circle |
| `eReportObjectFormulaDisplay` | 12 | Formula graphic |
| `eReportObjectSpider` | 13 | Spider axis system |
| `eReportObjectPieChart` | 14 | Pie chart |

## Python example

```python
dd.Report.NewLayout()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow,"MyArrow")
dd.MsgBoxDisp(oMyArrow.ObjectType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ObjectType_IRepArrowInt.htm`*
