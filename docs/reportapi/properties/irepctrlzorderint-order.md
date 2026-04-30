---
title: "IRepCtrlZOrderInt.Order"
description: "Specifies the order of an object in DIAdem REPORT."
---

# IRepCtrlZOrderInt.Order

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Order for ZOrder

Specifies the order of an object in DIAdem REPORT.

## Signature

```python
obj.Order
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    sOutput = sOutput + "Object type: " + oMyReportObj.ObjectType + "\t" + "Object name: " + oMyReportObj.Name  + "\t" + "Layer: " + oMyReportObj.Position.ZOrder.Order + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Order_IRepCtrlZOrderInt.htm`*
