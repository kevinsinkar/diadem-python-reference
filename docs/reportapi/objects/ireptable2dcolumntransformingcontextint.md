---
title: "IRepTable2DColumnTransformingContextInt"
description: "The Table2DColumnTransformingContext object provides information about a column of a 2D table for the channel transformation in DIAdem REPORT."
---

# IRepTable2DColumnTransformingContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Table2DColumnTransformingContext

The Table2DColumnTransformingContext object provides information about a column of a 2D table for the channel transformation in DIAdem REPORT.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(eReportObject2DTable,"My2DTable")
oMy2DTable.Position.ByBorder.Top = 30
oMy2DTable.Position.ByBorder.Bottom = 20
oMy2DTable.Position.ByBorder.Left = 20
oMy2DTable.Position.ByBorder.Right = 30
oMyColumn = oMy2DTable.Columns.Add(e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = eTableAlignmentDecimalPoint
oMyColumnTrans.Channel.Reference = "[1]/[2]"
oMy2DTable.Settings.UseChannelTransformation = True
oMyColumnTrans.OnChannelTransformation = "MyOnChannelTransformation"
dd.Report.Refresh()
```

```python
def MyOnChannelTransformation(TransformContext):
    oMyDataContext = TransformContext.DataContext
    ChnSum(oMyDataContext.ChannelNumberIn, oMyDataContext.ChannelNumberOut)  # Calculates the sum of the single values
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumntransformingcontextint-column/">Column</a> | <a href="../../properties/ireptable2dcolumntransformingcontextint-datacontext/">DataContext</a> | <a href="../../properties/ireptable2dcolumntransformingcontextint-sheet/">Sheet</a> | <a href="../../properties/ireptable2dcolumntransformingcontextint-table/">Table</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnTransformingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
