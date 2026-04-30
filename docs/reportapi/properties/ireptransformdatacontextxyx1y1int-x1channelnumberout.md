---
title: "IRepTransformDataContextXYX1Y1Int.X1ChannelNumberOut"
description: "Specifies the number of the x1-output channel for the Curve Transformation of a curve with a 4D vector display type in a 3D axis system in DIAdem REPORT."
---

# IRepTransformDataContextXYX1Y1Int.X1ChannelNumberOut

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: X1ChannelNumberOut for TransformDataContextXYX1Y1

Specifies the number of the x1-output channel for the Curve Transformation of a curve with a 4D vector display type in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.X1ChannelNumberOut
```

## Python example

```python
oMyShapeTrans, oMyArrowHeadTrans, oMySettingsTrans, oMyCurveLineExtensionTrans
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeVector, "My3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.VectorType = dd.e3DVectorType4D
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.XChannelEnd.Reference = "[3]/[3]"
oMyShape.YChannelEnd.Reference = "[3]/[4]"
oMySettings = oMyShape.Settings
oMySettings.EndCoordinateType = dd.e3DVectorEndCoordinateCartesianRelative
oMySettings.ScalingType = dd.e3DVectorScalingIsometric
oMyArrowHead = oMySettings.ArrowHead
oMyArrowHead.Type = dd.e3DVectorHeadVectorEnd
oMyCurveLineExtension = oMyShape.Extensions.CurveLine
oMyCurveLineExtension.Visible = True
oMy3DCurveTrans = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeVector, "My3DCurveTrans")
oMyShapeTrans = oMy3DCurveTrans.Shape
oMyShapeTrans.VectorType = dd.e3DVectorType4D
oMyShapeTrans.XChannel.Reference = "[3]/[1]"
oMyShapeTrans.YChannel.Reference = "[3]/[2]"
oMyShapeTrans.XChannelEnd.Reference = "[3]/[3]"
oMyShapeTrans.YChannelEnd.Reference = "[3]/[4]"
oMySettingsTrans = oMyShapeTrans.Settings
oMySettingsTrans.EndCoordinateType = dd.e3DVectorEndCoordinateCartesianRelative
oMySettingsTrans.ScalingType = dd.e3DVectorScalingIsometric
oMyArrowHeadTrans = oMySettingsTrans.ArrowHead
oMyArrowHeadTrans.Type = dd.e3DVectorHeadVectorEnd
oMyCurveLineExtensionTrans = oMyShapeTrans.Extensions.CurveLine
oMyCurveLineExtensionTrans.Visible = True
oMy3DAxisSystem.Settings.UseCurveTransformation = True
oMy3DCurveTrans.OnCurveTransformation = "MyOn3DCurveTransformation"
dd.Report.Refresh()
```

```python
def MyOn3DCurveTransformation(TransformContext):
    oMyDataContext = TransformContext.DataContext
    select_variable_0 = TransformContext.DataType
    if (select_variable_0 == dd.e3DCurveTransformDataTypeXYZ) :
        dd.ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnSmooth(oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut, 100, "symmetric") #Smooth the input channel and save the result as output channel
    elif (select_variable_0 == dd.e3DCurveTransformDataTypeXYX1Y1) :
        dd.ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.YChannelNumberIn ,oMyDataContext.YChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnLinScale (oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, 0) #Multiply the input channel with a value and save the result as output channel
        dd.ChnLinScale (oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, 0) #Multiply the input channel with a value and save the result as output channel
    elif (select_variable_0 == dd.e3DCurveTransformDataTypeXYZX1Y1Z1) :
        dd.ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnLinScale (oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, 0) #Multiply the input channel with a value and save the result as output channel
        dd.ChnLinScale (oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, 0) #Multiply the input channel with a value and save the result as output channel
        dd.ChnLinScale (oMyDataContext.Z1ChannelNumberIn, oMyDataContext.Z1ChannelNumberOut, 2, 0) #Multiply the input channel with a value and save the result as output channel
    elif (select_variable_0 == dd.e3DCurveTransformDataTypeCXCYCZ) :
        oMyDataContext.ConstXOut = oMyDataContext.ConstXIn + 20 #Add value to input constant
        oMyDataContext.ConstYOut = oMyDataContext.ConstYIn + 20 #Add value to input constant
        oMyDataContext.ConstZOut = oMyDataContext.ConstZIn + 20 #Add value to input constant
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_X1ChannelNumberOut_IRepTransformDataContextXYX1Y1Int.htm`*
