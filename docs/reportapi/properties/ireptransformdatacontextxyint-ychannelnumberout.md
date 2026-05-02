---
title: "IRepTransformDataContextXYInt.YChannelNumberOut"
description: "Specifies the number of the y-output channel for the Curve Transformation of a curve, whose data originates from an x-channel and a y-channel, in a 2D axis syst"
---

# IRepTransformDataContextXYInt.YChannelNumberOut

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannelNumberOut for TransformDataContextXY

Specifies the number of the y-output channel for the Curve Transformation of a curve, whose data originates from an x-channel and a y-channel, in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.YChannelNumberOut
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
oMy2DAxisSystem.Settings.UseCurveTransformation = True
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannelNumberOut_IRepTransformDataContextXYInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
