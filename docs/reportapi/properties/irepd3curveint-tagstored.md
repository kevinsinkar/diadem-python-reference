---
title: "IRepD3CurveInt.TagStored"
description: "Specifies a tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a"
---

# IRepD3CurveInt.TagStored

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TagStored for 3DCurve

Specifies a tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a program, for example, for special treatment of the object. The tag does not affect the behavior of the object. DIAdem saves this tag with the layout.

## Signature

```python
obj.TagStored
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        for oMyReportSubObj in oMyReportObj.Curves3D:
            oMyReportSubObj.TagStored = "Selected"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TagStored_IRepD3CurveInt.htm`*
