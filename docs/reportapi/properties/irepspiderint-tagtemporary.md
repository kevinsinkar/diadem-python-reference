---
title: "IRepSpiderInt.TagTemporary"
description: "Specifies a temporary tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such inform"
---

# IRepSpiderInt.TagTemporary

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TagTemporary for Spider

Specifies a temporary tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a program, for example, for special treatment of the object. The tag does not affect the behavior of the object. DIAdem does not save this tag with the layout.

## Signature

```python
obj.TagTemporary
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        oMyReportObj.TagTemporary = "Selected"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TagTemporary_IRepSpiderInt.htm`*
