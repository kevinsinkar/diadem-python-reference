---
title: "IRepReportOnDrawingInt.OnAxisSystem3DCurve"
description: "Specifies the user command that DIAdem REPORT executes when plotting a curve in a 3D axis system. The user command receives two parameters. The first parameter "
---

# IRepReportOnDrawingInt.OnAxisSystem3DCurve

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnAxisSystem3DCurve for DrawingEvents

Specifies the user command that DIAdem REPORT executes when plotting a curve in a 3D axis system. The user command receives two parameters. The first parameter corresponds to a D3CurveDrawingContext object and provides information about the 3D axis system and the worksheet into which DIAdem is plotting the curve. The second parameter corresponds to a 3DCurve object and provides information about the curve DIAdem is plotting. This curve is a temporary copy of the curve defined in the axis system. You can change this temporary curve any way you like. After plotting this curve, you can no longer access the temporary 3DCurve object. DIAdem REPORT saves this property with the layout. The user command is only executed if you use the Enable for CurveExpansionSettings property to enable the expansion mode.

## Signature

```python
obj.OnAxisSystem3DCurve
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnAxisSystem3DCurve_IRepReportOnDrawingInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
