---
title: "IRepReportEventsInt.Drawing"
description: "Returns the object in DIAdem REPORT that provides the events while a REPORT object is being plotted."
---

# IRepReportEventsInt.Drawing

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Drawing for Events

Returns the object in DIAdem REPORT that provides the events while a REPORT object is being plotted.

## Signature

```python
return_value = obj.Drawing
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
dd.Report.Events.Drawing.OnAxisSystem2DCurve = "MyOn2DCurveDrawEvent"

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

*Source: `ReportApi/properties/Report_property_Drawing_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
