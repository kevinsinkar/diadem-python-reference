---
title: "IRepTable2DColumnBaseInt"
description: "The 2DTableColumn object provides a column for a 2D table in DIAdem REPORT. The 2DTableColumn object corresponds to one of the following objects: 2DTableColumnC"
---

# IRepTable2DColumnBaseInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumn

The 2DTableColumn object provides a column for a 2D table in DIAdem REPORT. The 2DTableColumn object corresponds to one of the following objects: 2DTableColumnChannel (IRepTable2DColumnChannelInt) Channel 2DTableColumnExpression (IRepTable2DColumnExpressionInt) DIAdem expression 2DTableColumnText (IRepTable2DColumnTextInt) Text list 2DTableColumnVariable (IRepTable2DColumnVariableInt) Variables

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMySubObjects = oMyReportObj.Columns
        for oMySubObj in oMySubObjects:
            sOutput = sOutput + "Column type: " + oMySubObj.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnbaseint-index/">Index</a> | <a href="../../properties/ireptable2dcolumnbaseint-settings/">Settings</a> | <a href="../../properties/ireptable2dcolumnbaseint-tagstored/">TagStored</a> | <a href="../../properties/ireptable2dcolumnbaseint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireptable2dcolumnbaseint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-add/">Add</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-changetype/">ChangeType</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-copy/">Copy</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-item/">Item</a> | <a href="../ireptable2dcolumntransformingcontextint/">Table2DColumnTransformingContext</a>.<a href="../../properties/ireptable2dcolumntransformingcontextint-column/">Column</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnBaseInt.htm`*
