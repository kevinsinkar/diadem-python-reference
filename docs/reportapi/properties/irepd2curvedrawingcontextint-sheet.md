---
title: "IRepD2CurveDrawingContextInt.Sheet"
description: "Specifies the worksheet of the curve DIAdem is plotting in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveDrawingContextInt.Sheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sheet for D2CurveDrawingContext

Specifies the worksheet of the curve DIAdem is plotting in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Sheet
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Report.Events.OnDrawing2DAxisSystemCurve", "MyOn2DCurveDrawEvent")

def MyOn2DCurveDrawEvent(Context, CurrCurve):
    oMyAxis = Context.AxisSystem
    oMyCurve = CurrCurve
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

dd.MsgBox("Sheet: " + Context.Sheet.Name + "\r\n" + "Axis system: " + oMyAxis.Name + "Curve name: " + oMyCurve.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Sheet_IRepD2CurveDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
