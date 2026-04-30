---
title: "IRepPolarSelectedSubObjInt.Type"
description: "Specifies the type of the selected element in a polar axis system in DIAdem REPORT."
---

# IRepPolarSelectedSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for PolarSelectedElement

Specifies the type of the selected element in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarElementRadialAxis` | 0 | Radial axis |
| `ePolarElementRadialAxisNumbers` | 1 | Radial axis scale |
| `ePolarElementSectorNumbers` | 2 | Circle scale |
| `ePolarElementRadialAxisLabel` | 3 | Radial axis label |
| `ePolarElementCurve` | 4 | Curve |
| `ePolarElementCurveLegend` | 5 | Legend |

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        for oMySelectioned in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Object " + oMySelectioned.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepPolarSelectedSubObjInt.htm`*
