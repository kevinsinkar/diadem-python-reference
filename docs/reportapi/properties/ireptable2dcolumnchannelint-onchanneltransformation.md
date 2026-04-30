---
title: "IRepTable2DColumnChannelInt.OnChannelTransformation"
description: "Specifies the name of the user command that DIAdem REPORT executes to transform a curve while plotting. The parameter of the user command corresponds to a Table"
---

# IRepTable2DColumnChannelInt.OnChannelTransformation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnChannelTransformation for 2DTableColumnChannel

Specifies the name of the user command that DIAdem REPORT executes to transform a curve while plotting. The parameter of the user command corresponds to a Table2DColumnTransformingContext object and provides information about the 2D table, the worksheet, and the channels and their data type. Use this property only to manipulate the data of the input channels. REPORT objects such as the worksheet, the axis system, and the curves can only be accessed in read-only mode. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnChannelTransformation
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

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

*Source: `ReportApi/properties/Report_property_OnChannelTransformation_IRepTable2DColumnChannelInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
