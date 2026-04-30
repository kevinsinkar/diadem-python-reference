---
title: "IRepTable2DColumnTextInt.TagTemporary"
description: "Specifies a temporary tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such inform"
---

# IRepTable2DColumnTextInt.TagTemporary

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TagTemporary for 2DTableColumnText

Specifies a temporary tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a program, for example, for special treatment of the object. The tag does not affect the behavior of the object. DIAdem does not save this tag with the layout.

## Signature

```python
obj.TagTemporary
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMySubObjects = oMyReportObj.Columns
        for oMySubObj in oMySubObjects:
            oMySubObj.TagTemporary = "Column type: " + oMySubObj.Type
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TagTemporary_IRepTable2DColumnTextInt.htm`*
