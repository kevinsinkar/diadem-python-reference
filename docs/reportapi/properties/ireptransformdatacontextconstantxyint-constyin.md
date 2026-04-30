---
title: "IRepTransformDataContextConstantXYInt.ConstYIn"
description: "Specifies the values of the y-input constants for the curve transformation of a curve with the Constant or Coordinate display type in a 2D axis system in DIAdem"
---

# IRepTransformDataContextConstantXYInt.ConstYIn

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ConstYIn for TransformDataContextConstantXY

Specifies the values of the y-input constants for the curve transformation of a curve with the Constant or Coordinate display type in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.ConstYIn
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
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling
oMyXScaling.AutoScalingType = eAxisAutoScalingBeginEndManual
oMyXScaling.Begin = 0
oMyXScaling.End = 70
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = eAxisAutoScalingBeginEndManual
oMyYScaling.Begin = 0
oMyYScaling.End = 70
oMyCurveConstOrg = oMy2DAxisSystem.Curves2D.Add(e2DShapeConstant, "MyOrgConstant")
oMyCurveConstOrg.Shape.XConstant.Reference = 10
oMyCurveConstOrg.Shape.YConstant.Reference = 20
oMyCurveConstTrans = oMy2DAxisSystem.Curves2D.Add(e2DShapeConstant, "MyTransConstant")
oMyCurveConstTrans.Shape.XConstant.Reference = 10
oMyCurveConstTrans.Shape.YConstant.Reference = 20
oMy2DAxisSystem.Settings.UseCurveTransformation = TRUE
oMyCurveConstTrans.OnCurveTransformation = "MyOnCurveTransformation"
dd.Report.Refresh()
```

```python
def MyOnCurveTransformation(Context):
    oMyDataContext = Context.DataContext
    # select Context.DataType
    # case e2DCurveTransformDataTypeXY
    ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut) 'Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut, 100, "symmetric") 'Smooth the input channel and save the result as output channel
    # case e2DCurveTransformDataTypeXYY1
    ChnCopy  (oMyDataContext.XChannelNumberIn ,oMyDataContext.XChannelNumberOut) 'Copy the input channel into the output channel
    ChnSmooth(oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    ChnSmooth(oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, "symmetric") 'Smooth the input channel and save the result as output channel
    # case e2DCurveTransformDataTypeCXCY
    oMyDataContext.ConstXOut = oMyDataContext.ConstXIn + 20
    oMyDataContext.ConstYOut = oMyDataContext.ConstYIn + 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ConstYIn_IRepTransformDataContextConstantXYInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
