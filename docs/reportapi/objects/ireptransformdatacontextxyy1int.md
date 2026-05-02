---
title: "IRepTransformDataContextXYY1Int"
description: "The TransformDataContextXYY1 object provides the input and output channels for the curve transformation of a curve as an object in a 2D axis system in DIAdem RE"
---

# IRepTransformDataContextXYY1Int

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: TransformDataContextXYY1

The TransformDataContextXYY1 object provides the input and output channels for the curve transformation of a curve as an object in a 2D axis system in DIAdem REPORT. Use the TransformDataContextXYY1 object for all 2D display types in which the data originates from an x-channel, a y-channel, and a y1 channel. The user command receives the TransformDataContextXYY1 object as a parameter. Use the curve transformation user command only to manipulate the values of temporary copies of the input channels. REPORT objects such as the worksheet, the axis system, and the curves can only be accessed in read-only mode.

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
oMy2DCurveOrg = oMy2DAxisSystem.Curves2D.Add(e2DShapeFilledArea, "MyOrgCurve")
oMy2DCurveOrg.Shape.XChannel.Reference = "[2]/[1]"
oMy2DCurveOrg.Shape.YChannel.Reference = "[2]/[2]"
oMy2DCurveOrg.Shape.YChannelDifferential.Reference = "[2]/[3]"
oMy2DCurveOrg.Shape.Settings.FillEffects.Color.SetPredefinedColor(eColorIndexBlue)
oMy2DCurveOrg.Shape.Settings.FillEffects.Color.Transparency = 50
oMy2DCurveTrans = oMy2DAxisSystem.Curves2D.Add(e2DShapeFilledArea, "MyTransCurve")
oMy2DCurveTrans.Shape.XChannel.Reference = "[2]/[1]"
oMy2DCurveTrans.Shape.YChannel.Reference = "[2]/[2]"
oMy2DCurveTrans.Shape.YChannelDifferential.Reference = "[2]/[3]"
oMy2DCurveTrans.Shape.Settings.FillEffects.Color.SetPredefinedColor(eColorIndexRed)
oMy2DCurveTrans.Shape.Settings.FillEffects.Color.Transparency = 50
oMy2DAxisSystem.Settings.UseCurveTransformation = TRUE
oMy2DCurveTrans.OnCurveTransformation = "MyOnCurveTransformation"
dd.Report.Refresh()
```

```python
def MyOnCurveTransformation(Context):
    oMyDataContext = Context.DataContext
    # select Context.DataType
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
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptransformdatacontextxyy1int-xchannelnumberin/">XChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyy1int-xchannelnumberout/">XChannelNumberOut</a> | <a href="../../properties/ireptransformdatacontextxyy1int-y1channelnumberin/">Y1ChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyy1int-y1channelnumberout/">Y1ChannelNumberOut</a> | <a href="../../properties/ireptransformdatacontextxyy1int-ychannelnumberin/">YChannelNumberIn</a> | <a href="../../properties/ireptransformdatacontextxyy1int-ychannelnumberout/">YChannelNumberOut</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTransformDataContextXYY1Int.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
