---
title: "IRepD3CurveInt.OnCurveTransformation"
description: "Specifies the name of the user command that DIAdem REPORT executes to transform a curve while plotting. The parameter of the user command corresponds to a D3Cur"
---

# IRepD3CurveInt.OnCurveTransformation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnCurveTransformation for 3DCurve

Specifies the name of the user command that DIAdem REPORT executes to transform a curve while plotting. The parameter of the user command corresponds to a D3CurveTransformingContext object and provides information about the 3D axis system, the worksheet, and the channels and their data type. Use this property only to manipulate the data of the input channels. REPORT objects such as the worksheet, the axis system, and the curves can only be accessed in read-only mode. Use the curve transformation function to modify the displayed channels while they are being plotted. DIAdem does not modify the original data. The transformed channels have the same display format as the original channels. For example, you cannot create a numeric channel from a time channel using the curve transformation. If you do not specify an x-channel and the y-channel is an xy-channel and you have selected the setting When plotting xy-channels, determine x-channel automatically if not populated in the General DIAdem Settings , you can also transform the x-channel that belongs to the y-channel. The display format remains the same. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnCurveTransformation
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
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(e3DShapeSurface, "My3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMy3DCurveTrans = oMy3DAxisSystem.Curves3D.Add(e3DShapeSurface, "My3DCurveTrans")
oMyShape = oMy3DCurveTrans.Shape
oMyShape.DataStructure = e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMy3DAxisSystem.Settings.UseCurveTransformation = TRUE
oMy3DCurveTrans.OnCurveTransformation = "MyOn3DCurveTransformation"
dd.Report.Refresh()
```

```python
def MyOn3DCurveTransformation(TransformContext):
    oMyDataContext = TransformContext.DataContext
    # select TransformContext.DataType
    # case e3DCurveTransformDataTypeXYZ
    ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut) 'Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut, 100, "symmetric") 'Smooth the input channel and save the result as output channel
    # case e3DCurveTransformDataTypeXYX1Y1
    ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn ,oMyDataContext.YChannelNumberOut) 'Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    ChnSmooth(oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    # case e3DCurveTransformDataTypeXYZX1Y1Z1
    ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut) 'Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    ChnSmooth(oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    ChnSmooth(oMyDataContext.Z1ChannelNumberIn, oMyDataContext.Z1ChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    # case e3DCurveTransformDataTypeCXCYCZ
    ChnCopy  (oMyDataContext.ConstXIn, oMyDataContext.ConstXOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.ConstYIn, oMyDataContext.ConstYOut) 'Copy the input channel into the output channel
    oMyDataContext.ConstZOut = oMyDataContext.ConstZIn + 2
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnCurveTransformation_IRepD3CurveInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
