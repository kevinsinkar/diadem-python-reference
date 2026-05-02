---
title: "IRepD2CurveInt.OnCurveTransformation"
description: "Is triggered in DIAdem REPORT to transform a curve that is being plotted. The event starts the user command that you assigned to the OnCurveTransformation prope"
---

# IRepD2CurveInt.OnCurveTransformation

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnCurveTransformation for 2DCurve

Is triggered in DIAdem REPORT to transform a curve that is being plotted. The event starts the user command that you assigned to the OnCurveTransformation property. The user command receives a parameter. The parameter of the user command corresponds to a D2CurveTransformingContext object and provides information about the 2D axis system, the worksheet, and the channels and their data type. Access the REPORT objects such as the worksheet, the 2D axis system, and the curves in read-only mode. Use the curve transformation function to modify the displayed channels while they are being plotted. DIAdem does not modify the original data. The transformed channels have the same display format as the original channels. For example, you cannot create a numeric channel from a time channel using the curve transformation. If you do not specify an x-channel and the y-channel is an xy-channel and you have selected the setting When plotting xy-channels, determine x-channel automatically if not populated in the General DIAdem Settings , you can also transform the x-channel that belongs to the y-channel. The display format remains the same. Refer to Working with Events in DIAdem for more information on events in DIAdem.

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnCurveTransformation_IRepD2CurveInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
