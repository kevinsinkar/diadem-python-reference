---
title: "IRepSpiderSelectedSubObjInt.Name"
description: "Specifies the name of the selected object in a spider axis system in DIAdem REPORT."
---

# IRepSpiderSelectedSubObjInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for SpiderSelectedElement

Specifies the name of the selected object in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Name
```

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
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepSpiderSelectedSubObjInt.htm`*
