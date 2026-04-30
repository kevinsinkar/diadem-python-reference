---
title: "IRepTable2DColumnVariableInt.Index"
description: "Specifies the index of a 2D table column in DIAdem REPORT. The table column takes its contents from a variable."
---

# IRepTable2DColumnVariableInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for 2DTableColumnVariable

Specifies the index of a 2D table column in DIAdem REPORT. The table column takes its contents from a variable.

## Signature

```python
obj.Index
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMySubObjects = oMyReportObj.Columns
        for oMySubObj in oMySubObjects:
            sOutput = sOutput + "Column index: " + oMySubObj.Index + "\t" + "Column type: " + oMySubObj.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepTable2DColumnVariableInt.htm`*
