---
title: "IRepSpiderSelectedSubObjInt.Type"
description: "Specifies the type of the selected element in a spider axis system in DIAdem REPORT."
---

# IRepSpiderSelectedSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for SpiderSelectedElement

Specifies the type of the selected element in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderElementAxis` | 0 | Axis |
| `eSpiderElementAxisNumbers` | 1 | Axis scale labels |
| `eSpiderElementAxisLabel` | 2 | Show/hide |
| `eSpiderElementCurve` | 3 | Curve |
| `eSpiderElementCurveLegend` | 4 | Legend |

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepSpiderSelectedSubObjInt.htm`*
