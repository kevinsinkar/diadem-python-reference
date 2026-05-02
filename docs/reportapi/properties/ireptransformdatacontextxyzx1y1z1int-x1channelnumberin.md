---
title: "IRepTransformDataContextXYZX1Y1Z1Int.X1ChannelNumberIn"
description: "Specifies the number of the x1-input channel for the Curve Transformation of a curve with a 6D vector display type in a 3D axis system in DIAdem REPORT."
---

# IRepTransformDataContextXYZX1Y1Z1Int.X1ChannelNumberIn

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: X1ChannelNumberIn for TransformDataContextXYZX1Y1Z1

Specifies the number of the x1-input channel for the Curve Transformation of a curve with a 6D vector display type in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.X1ChannelNumberIn
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
oMyShape.VectorType = e3DVectorType6D
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyShape.XChannelEnd.Reference = "[3]/[4]"
oMyShape.YChannelEnd.Reference = "[3]/[5]"
oMyShape.ZChannelEnd.Reference = "[3]/[6]"
oMySettings = oMyShape.Settings
oMySettings.EndCoordinateType = e3DVectorEndCoordinateCartesianRelative
oMySettings.ScalingType = e3DVectorScalingIsometric
oMyArrowHead = oMySettings.ArrowHead
oMyArrowHead.Type = e3DVectorHeadVectorEnd
oMyCurveLineExtension = oMyShape.Extensions.CurveLine
oMyCurveLineExtension.Visible = True
oMy3DCurveTrans = oMy3DAxisSystem.Curves3D.Add(e3DShapeVector, "My3DCurveTrans")
oMyShapeTrans = oMy3DCurveTrans.Shape
oMyShapeTrans.VectorType = e3DVectorType6D
oMyShapeTrans.XChannel.Reference = "[3]/[1]"
oMyShapeTrans.YChannel.Reference = "[3]/[2]"
oMyShapeTrans.ZChannel.Reference = "[3]/[3]"
oMyShapeTrans.XChannelEnd.Reference = "[3]/[4]"
oMyShapeTrans.YChannelEnd.Reference = "[3]/[5]"
oMyShapeTrans.ZChannelEnd.Reference = "[3]/[6]"
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_X1ChannelNumberIn_IRepTransformDataContextXYZX1Y1Z1Int.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
