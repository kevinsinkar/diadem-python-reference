---
title: "IRepTransformDataContextXInt.ChannelNumberIn"
description: "Specifies the number of the input channel for the channel transformation in a 2D table in DIAdem REPORT."
---

# IRepTransformDataContextXInt.ChannelNumberIn

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ChannelNumberIn for TransformDataContextX

Specifies the number of the input channel for the channel transformation in a 2D table in DIAdem REPORT.

## Signature

```python
obj.ChannelNumberIn
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
    ChnSum(oMyDataContext.ChannelNumberIn, oMyDataContext.ChannelNumberOut)  # Calculates the sum of the channel values
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ChannelNumberIn_IRepTransformDataContextXInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
