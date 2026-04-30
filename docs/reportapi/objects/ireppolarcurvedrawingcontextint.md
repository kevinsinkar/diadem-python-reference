---
title: "IRepPolarCurveDrawingContextInt"
description: "The PolarCurveDrawingContext object provides information about the polar axis system and the worksheet into which DIAdem REPORT is plotting the current curve."
---

# IRepPolarCurveDrawingContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarCurveDrawingContext

The PolarCurveDrawingContext object provides information about the polar axis system and the worksheet into which DIAdem REPORT is plotting the current curve.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.Drawing.OnPolarSystemCurve = "MyOnPolarCurveDrawEvent"

def MyOnPolarCurveDrawEvent(Context, CurrCurve):
    oMyAxis = Context.PolarSystem
    oMyCurve = CurrCurve
    # select oMyCurve.ShapeType
    # case ePolarShapeLine
    oMyCurve.Shape.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case ePolarShapeLineAndPoints
    oMyCurve.Shape.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case ePolarShapeSpikes
    oMyCurve.Shape.Spike.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case ePolarShapeDifferential
    oMyCurve.Shape.DifferentialLine.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)

dd.MsgBox("Sheet: " + Context.Sheet.Name + VBCrLf + "Axis system: " + oMyAxis.Name + "Curve name: " + oMyCurve.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarcurvedrawingcontextint-polarsystem/">PolarSystem</a> | <a href="../../properties/ireppolarcurvedrawingcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarCurveDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
