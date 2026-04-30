---
title: "IRepReportOnDrawingInt.OnAxisSystem2DCurve"
description: "Is triggered in DIAdem REPORT while a curve in a 2D axis system is being plotted. The event starts the user command that you assigned to the OnAxisSystem2D for "
---

# IRepReportOnDrawingInt.OnAxisSystem2DCurve

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnAxisSystem2DCurve for DrawingEvents

Is triggered in DIAdem REPORT while a curve in a 2D axis system is being plotted. The event starts the user command that you assigned to the OnAxisSystem2D for DrawingEvents property. The user command receives two parameters. The first parameter corresponds to a D2CurveDrawingContext object and provides information about the 2D axis system and the worksheet into which DIAdem is plotting the curve. The second parameter corresponds to a 2DCurve object and provides information about the curve DIAdem is plotting. This curve is a temporary copy of the curve defined in the axis system. You can change this temporary curve any way you like. After plotting this curve, you can no longer access the temporary 2DCurve object. DIAdem executes the user command that you assigned to the OnAxisSystem2D for DrawingEvents property, just before DIAdem plots the curves. At this point in time DIAdem has already resolved all channel references, and has already expanded the curves and executed actions such as transferring the curve color to the markers. If you, for example, set the curve color in this user command, the user command must also adapt all the correlated colors. DIAdem REPORT saves this property with the layout. The user command is only executed if you use the Enable for CurveExpansionSettings property to enable the expansion mode. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnAxisSystem2DCurve
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.Report.Events.Drawing.OnAxisSystem2DCurve", "MyOn2DCurveDrawEvent")

def MyOn2DCurveDrawEvent(Context, CurrCurve):
    oMyAxis = Context.AxisSystem
    oMyCurve = CurrCurve
    dd.Report.Settings.CurveExpansion.Enable = True
    # select oMyCurve.ShapeType
    # case e2DShapeLine
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeLineAndPoints
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeSpikes
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeBars
    oMyCurve.Shape.Settings.BorderLine.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeOutlineBars
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeDifferential
    oMyCurve.Shape.Settings.BorderLine.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeConstant
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeSpikesHorizontal
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeBarsHorizontal
    oMyCurve.Shape.Settings.BorderLine.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeOutlineBarsHorizontal
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeSpecialCombination
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeCoordinate
    oMyCurve.Shape.Settings.MarkerBorderLine.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e2DShapeFilledArea
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)

dd.MsgBox("Sheet: " + Context.Sheet.Name + VBCrLf + "Axis system: " + oMyAxis.Name + "Curve name: " + oMyCurve.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnAxisSystem2DCurve_IRepReportOnDrawingInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
