---
title: "IRepSpiderSelectedSubObjInt"
description: "The SpiderSelectedElement object provides a selected element in a spider axis system in DIAdem REPORT."
---

# IRepSpiderSelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderSelectedElement

The SpiderSelectedElement object provides a selected element in a spider axis system in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspiderselectedsubobjint-name/">Name</a> | <a href="../../properties/irepspiderselectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/spiderselectedelements/">SpiderSelectedElements</a>.<a href="../../methods/irepspiderselectedsubobjectslistint-addspider/">AddSpider</a> | <a href="../../collections/spiderselectedelements/">SpiderSelectedElements</a>.<a href="../../methods/irepspiderselectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderSelectedSubObjInt.htm`*
