---
title: "IRepTable2DColumnChannelInt.IsExpanded"
description: "Specifies whether a column in a 2D table in DIAdem REPORT is expanded. You must not change the channel reference of an expanded column. You can only change the "
---

# IRepTable2DColumnChannelInt.IsExpanded

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: IsExpanded for 2DTableColumnChannel

Specifies whether a column in a 2D table in DIAdem REPORT is expanded. You must not change the channel reference of an expanded column. You can only change the channel reference if the column is a Table2DColumnDrawingContext object.

## Signature

```python
bIsExpanded = Object.IsExpanded()
```

## Python example

```python
sOutput = ""
dd.Report.Settings.CurveExpansion.Expand()
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMyColumns = oMyReportObj.Columns
        print ("Number of columns: " , oMyColumns.Count)
        for oMyColumn in oMyColumns:
            sOutput = sOutput + "Object index: " + oMyColumn.Index + "\t" + "IsExpanded: " + oMyColumn.IsExpanded + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_IsExpanded_IRepTable2DColumnChannelInt.htm`*
