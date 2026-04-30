---
title: "IRepTransformDataContextConstantXYZInt"
description: "The TransformDataContextConstantXYZ object provides the input and output constants for the curve transformation of a curve with the Coordinate display type as a"
---

# IRepTransformDataContextConstantXYZInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: TransformDataContextConstantXYZ

The TransformDataContextConstantXYZ object provides the input and output constants for the curve transformation of a curve with the Coordinate display type as an object in a 3D axis system in DIAdem REPORT. The user command receives the TransformDataContextConstantXYZ object as a parameter. Use the curve transformation user command only to manipulate the values of temporary copies of the input channels. REPORT objects such as the worksheet, the axis system, and the curves can only be accessed in read-only mode.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(e3DShapeCoordinate, "My3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XCoordinate.Reference = 10
oMyShape.YCoordinate.Reference = 20
oMyShape.ZCoordinate.Reference = 30
oMy3DCurveTrans = oMy3DAxisSystem.Curves3D.Add(e3DShapeCoordinate, "My3DCurveTrans")
oMyShapeTrans = oMy3DCurveTrans.Shape
oMyShapeTrans.XCoordinate.Reference = 10
oMyShapeTrans.YCoordinate.Reference = 20
oMyShapeTrans.ZCoordinate.Reference = 30
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
    ChnLinScale (oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, 0) 'Multiply the input channel with a value and save the result as output channel
    ChnLinScale (oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, 0) 'Multiply the input channel with a value and save the result as output channel
    # case e3DCurveTransformDataTypeXYZX1Y1Z1
    ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut) 'Copy the input channel into the output channel
    ChnCopy  (oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut) 'Copy the input channel into the output channel
    ChnLinScale (oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, 0) 'Multiply the input channel with a value and save the result as output channel
    ChnLinScale (oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, 0) 'Multiply the input channel with a value and save the result as output channel
    ChnLinScale (oMyDataContext.Z1ChannelNumberIn, oMyDataContext.Z1ChannelNumberOut, 2, 0) 'Multiply the input channel with a value and save the result as output channel
    # case e3DCurveTransformDataTypeCXCYCZ
    oMyDataContext.ConstXOut = oMyDataContext.ConstXIn + 20 'Add value to input constant
    oMyDataContext.ConstYOut = oMyDataContext.ConstYIn + 20 'Add value to input constant
    oMyDataContext.ConstZOut = oMyDataContext.ConstZIn + 20 'Add value to input constant
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptransformdatacontextconstantxyzint-constxin/">ConstXIn</a> | <a href="../../properties/ireptransformdatacontextconstantxyzint-constxout/">ConstXOut</a> | <a href="../../properties/ireptransformdatacontextconstantxyzint-constyin/">ConstYIn</a> | <a href="../../properties/ireptransformdatacontextconstantxyzint-constyout/">ConstYOut</a> | <a href="../../properties/ireptransformdatacontextconstantxyzint-constzin/">ConstZIn</a> | <a href="../../properties/ireptransformdatacontextconstantxyzint-constzout/">ConstZOut</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepTransformDataContextConstantXYZInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
