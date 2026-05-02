---
title: "IRepTransformDataContextXYX1Y1Int"
description: "The TransformDataContextConstantXYZ object provides the input and output channels for the curve transformation of a curve with the 4D Vector display as an objec"
---

# IRepTransformDataContextXYX1Y1Int

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: TransformDataContextXYX1Y1

The TransformDataContextConstantXYZ object provides the input and output channels for the curve transformation of a curve with the 4D Vector display as an object type in a 3D axis system in DIAdem REPORT. The user command receives the TransformDataContextXYX1Y1 object as a parameter. Use the curve transformation user command only to manipulate the values of temporary copies of the input channels. REPORT objects such as the worksheet, the axis system, and the curves can only be accessed in read-only mode.

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
dd.Data.Root.Clear()
DataFileLoad(DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(e3DShapeVector, "My3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.VectorType = e3DVectorType4D
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.XChannelEnd.Reference = "[3]/[3]"
oMyShape.YChannelEnd.Reference = "[3]/[4]"
oMySettings = oMyShape.Settings
oMySettings.EndCoordinateType = e3DVectorEndCoordinateCartesianRelative
oMySettings.ScalingType = e3DVectorScalingIsometric
oMyArrowHead = oMySettings.ArrowHead
oMyArrowHead.Type = e3DVectorHeadVectorEnd
oMyCurveLineExtension = oMyShape.Extensions.CurveLine
oMyCurveLineExtension.Visible = True
oMy3DCurveTrans = oMy3DAxisSystem.Curves3D.Add(e3DShapeVector, "My3DCurveTrans")
oMyShapeTrans = oMy3DCurveTrans.Shape
oMyShapeTrans.VectorType = e3DVectorType4D
oMyShapeTrans.XChannel.Reference = "[3]/[1]"
oMyShapeTrans.YChannel.Reference = "[3]/[2]"
oMyShapeTrans.XChannelEnd.Reference = "[3]/[3]"
oMyShapeTrans.YChannelEnd.Reference = "[3]/[4]"
oMySettingsTrans = oMyShapeTrans.Settings
oMySettingsTrans.EndCoordinateType = e3DVectorEndCoordinateCartesianRelative
oMySettingsTrans.ScalingType = e3DVectorScalingIsometric
oMyArrowHeadTrans = oMySettingsTrans.ArrowHead
oMyArrowHeadTrans.Type = e3DVectorHeadVectorEnd
oMyCurveLineExtensionTrans = oMyShapeTrans.Extensions.CurveLine
oMyCurveLineExtensionTrans.Visible = True
oMy3DAxisSystem.Settings.UseCurveTransformation = TRUE
oMy3DCurveTrans.OnCurveTransformation = "MyOn3DCurveTransformation"
dd.Report.Refresh()
```

```python
def MyOn3DCurveTransformation(TransformContext):
    oMyDataContext = TransformContext.DataContext
    # select TransformContext.DataType
    # case e3DCurveTransformDataTypeXYZ
    ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut)  # Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut)  # Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut, 100, "symmetric")  # Smooth the input channel and save the result as output channel
    # case e3DCurveTransformDataTypeXYX1Y1
    ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut)  # Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn ,oMyDataContext.YChannelNumberOut)  # Copy the input channel into the output channel
    ChnLinScale (oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, 0)  # Multiply the input channel with a value and save the result as output channel
    ChnLinScale (oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, 0)  # Multiply the input channel with a value and save the result as output channel
    # case e3DCurveTransformDataTypeXYZX1Y1Z1
    ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut)  # Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut)  # Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut)  # Copy the input channel into the output channel
    ChnLinScale (oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, 0)  # Multiply the input channel with a value and save the result as output channel
    ChnLinScale (oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, 0)  # Multiply the input channel with a value and save the result as output channel
    ChnLinScale (oMyDataContext.Z1ChannelNumberIn, oMyDataContext.Z1ChannelNumberOut, 2, 0)  # Multiply the input channel with a value and save the result as output channel
    # case e3DCurveTransformDataTypeCXCYCZ
    oMyDataContext.ConstXOut = oMyDataContext.ConstXIn + 20  # Add value to input constant
    oMyDataContext.ConstYOut = oMyDataContext.ConstYIn + 20  # Add value to input constant
    oMyDataContext.ConstZOut = oMyDataContext.ConstZIn + 20  # Add value to input constant
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptransformdatacontextxyx1y1int-x1channelnumberin/">X1ChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-x1channelnumberout/">X1ChannelNumberOut</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-xchannelnumberin/">XChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-xchannelnumberout/">XChannelNumberOut</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-y1channelnumberin/">Y1ChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-y1channelnumberout/">Y1ChannelNumberOut</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-ychannelnumberin/">YChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyx1y1int-ychannelnumberout/">YChannelNumberOut</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curvetransformingcontextint/">D2CurveTransformingContext</a>.<a href="../../properties/irepd2curvetransformingcontextint-datacontext/">DataContext</a> | <a href="../irepd3curvetransformingcontextint/">D3CurveTransformingContext</a>.<a href="../../properties/irepd3curvetransformingcontextint-datacontext/">DataContext</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTransformDataContextXYX1Y1Int.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
