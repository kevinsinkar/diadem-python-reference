---
title: "IRepBaseCtrlInt.Index"
description: "Returns the index of an object in DIAdem REPORT. If you change the ZOrder property of an object, you also change the indexes of all objects."
---

# IRepBaseCtrlInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for ReportObject

Returns the index of an object in DIAdem REPORT. If you change the ZOrder property of an object, you also change the indexes of all objects.

## Signature

```python
obj.Index
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    sOutput = sOutput + "Object name: " + oMyReportObj.Name + "\t" + " Index: " + oMyReportObj.Index + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepBaseCtrlInt.htm`*
