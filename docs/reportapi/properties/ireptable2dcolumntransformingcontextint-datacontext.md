---
title: "IRepTable2DColumnTransformingContextInt.DataContext"
description: "Specifies the number of the input and output channel for the channel transformation in a column of a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnTransformingContextInt.DataContext

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DataContext for Table2DColumnTransformingContext

Specifies the number of the input and output channel for the channel transformation in a column of a 2D table in DIAdem REPORT.

## Signature

```python
return_value = obj.DataContext
```

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
oMyColumnTrans = oMy2DTable.Columns.Add(e2DTableColumnChannel)
oMyColumnTrans.Channel.Reference = "[1]/[2]"
oMy2DTable.Settings.UseChannelTransformation = True
oMyColumnTrans.OnChannelTransformation = "MyOnChannelTransformation"
dd.Report.Refresh()
```

```python
def MyOnChannelTransformation(TransformContext):
    oMyDataContext = TransformContext.DataContext
    ChnSum(oMyDataContext.ChannelNumberIn, oMyDataContext.ChannelNumberOut) 'Calculates the sum of the single values
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DataContext_IRepTable2DColumnTransformingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
