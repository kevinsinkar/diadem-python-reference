---
title: "IRepBaseTransformDataContextInt"
description: "The TransformDataContext object provides the input and output channels and the the input and output constants as objects for the curve transformation in a user "
---

# IRepBaseTransformDataContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: TransformDataContext

The TransformDataContext object provides the input and output channels and the the input and output constants as objects for the curve transformation in a user command in DIAdem REPORT. The user command receives the TransformDataContext object as a parameter. Use the curve transformation user command only to manipulate the values of temporary copies of the input channels. REPORT objects such as the worksheet, the axis system, and the curves can only be accessed in read-only mode.

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
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurveOrg = oMy2DaxisSystem.Curves2D.Add(e2DShapeLine, "MyOrgDCurve")
oMy2DCurveOrg.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurveOrg.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurveTrans = oMy2DaxisSystem.Curves2D.Add(e2DShapeLine, "MyTransCurve")
oMy2DCurveTrans.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurveTrans.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurveOrg.Shape.Settings.Line.Color.SetPredefinedColor(eColorIndexBlue)
oMy2DCurveTrans.Shape.Settings.Line.Color.SetPredefinedColor(eColorIndexRed)
oMy2DAxisSystem.Settings.UseCurveTransformation = TRUE
oMy2DCurveTrans.OnCurveTransformation = "MyOnCurveTransformation"
dd.Report.Refresh()
```

```python
def MyOnCurveTransformation(TransformDataContext):
    oMyDataContext = TransformDataContext.DataContext
    # select TransformDataContext.DataType
    # case e2DCurveTransformDataTypeXY
    ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut)  # Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut, 100, "symmetric")  # Smooth the input channel and save the result as output channel
    # case e2DCurveTransformDataTypeXYY1
    ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut)  # Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut, 2, "symmetric")  # Smooth the input channel and save the result as output channel
    ChnSmooth(oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, "symmetric")  # Smooth the input channel and save the result as output channel
    # case e2DCurveTransformDataTypeCXCY
    oMyDataContext.ConstXOut = oMyDataContext.ConstXIn + 2
    oMyDataContext.ConstYOut = oMyDataContext.ConstYIn + 2
```

## Members

<div markdown="1">
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

*Source: `ReportApi/Objects/Report_Objects_IRepBaseTransformDataContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
