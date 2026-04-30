---
title: "IRepD3CurveTransformingContextInt"
description: "The D3CurveTransformingContext object provides information about a 3D curve for curve transformation in DIAdem REPORT."
---

# IRepD3CurveTransformingContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: D3CurveTransformingContext

The D3CurveTransformingContext object provides information about a 3D curve for curve transformation in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "My3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMy3DCurveTrans = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "My3DCurveTrans")
oMyShape = oMy3DCurveTrans.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
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
        dd.ChnSmooth(oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, "symmetric") #Smooth the input channel and save the result as output channel
        dd.ChnSmooth(oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, "symmetric") #Smooth the input channel and save the result as output channel
    elif (select_variable_0 == dd.e3DCurveTransformDataTypeXYZX1Y1Z1) :
        dd.ChnCopy  (oMyDataContext.XChannelNumberIn, oMyDataContext.XChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.YChannelNumberIn, oMyDataContext.YChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.ZChannelNumberIn, oMyDataContext.ZChannelNumberOut) #Copy the input channel into the output channel
        dd.ChnSmooth(oMyDataContext.X1ChannelNumberIn, oMyDataContext.X1ChannelNumberOut, 2, "symmetric") #Smooth the input channel and save the result as output channel
        dd.ChnSmooth(oMyDataContext.Y1ChannelNumberIn, oMyDataContext.Y1ChannelNumberOut, 2, "symmetric") #Smooth the input channel and save the result as output channel
        dd.ChnSmooth(oMyDataContext.Z1ChannelNumberIn, oMyDataContext.Z1ChannelNumberOut, 2, "symmetric") #Smooth the input channel and save the result as output channel
    elif (select_variable_0 == dd.e3DCurveTransformDataTypeCXCYCZ) :
        dd.ChnCopy  (oMyDataContext.ConstXIn, oMyDataContext.ConstXOut) #Copy the input channel into the output channel
        dd.ChnCopy  (oMyDataContext.ConstYIn, oMyDataContext.ConstYOut) #Copy the input channel into the output channel
        oMyDataContext.ConstZOut = oMyDataContext.ConstZIn + 2
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3curvetransformingcontextint-axissystem/">AxisSystem</a> | <a href="../../properties/irepd3curvetransformingcontextint-curve/">Curve</a> | <a href="../../properties/irepd3curvetransformingcontextint-datacontext/">DataContext</a> | <a href="../../properties/irepd3curvetransformingcontextint-datatype/">DataType</a> | <a href="../../properties/irepd3curvetransformingcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3CurveTransformingContextInt.htm`*
