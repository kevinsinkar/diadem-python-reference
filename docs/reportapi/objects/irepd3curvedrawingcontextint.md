---
title: "IRepD3CurveDrawingContextInt"
description: "The D3CurveDrawingContext object provides information about the 3D axis system and the worksheet into which DIAdem REPORT is plotting the current curve."
---

# IRepD3CurveDrawingContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: D3CurveDrawingContext

The D3CurveDrawingContext object provides information about the 3D axis system and the worksheet into which DIAdem REPORT is plotting the current curve.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.Drawing.OnAxisSystem3DCurve = "MyOn3DCurveDrawEvent"

def MyOn3DCurveDrawEvent(Context, CurrCurve):
    oMyAxis = Context.AxisSystem
    oMyCurve = CurrCurve
    # select oMyCurve.ShapeType
    # case e3DShapeSurface
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeIsolines
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeWaterfall
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeBars
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeMatrix2D
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeSpikes
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeLine
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeVector
    oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapePoints
    oMyCurve.Shape.Settings.Marker.Line.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
    # case e3DShapeCharacteristicDiagram
    oMyCurve.Shape.Settings.SurfaceColorType =e3DCharacteristicSurfaceColorGlobalColorPalette3
    # case e3DShapeCoordinate
    oMyCurve.Shape.Settings.MarkerLine.Color.SetPredefinedColor(ePredefinedColorDarkTurquoise)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3curvedrawingcontextint-axissystem/">AxisSystem</a> | <a href="../../properties/irepd3curvedrawingcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3CurveDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
