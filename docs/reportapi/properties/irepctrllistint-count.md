---
title: "IRepCtrlListInt.Count"
description: "Returns the number of objects in a worksheet in DIAdem REPORT."
---

# IRepCtrlListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for ReportObjects

Returns the number of objects in a worksheet in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyObjects = dd.Report.ActiveSheet.Objects
for i in range( 1, oMyObjects.Count+1):
    sOutput = sOutput + "Object type: " + oMyObjects.Item(i).ObjectType + "\t" + "Element name: " + oMyObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepCtrlListInt.htm`*
