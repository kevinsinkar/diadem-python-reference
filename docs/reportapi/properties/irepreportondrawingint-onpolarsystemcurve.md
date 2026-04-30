---
title: "IRepReportOnDrawingInt.OnPolarSystemCurve"
description: "Specifies the user command that DIAdem REPORT executes when plotting a curve in a polar axis system. The user command receives two parameters. The first paramet"
---

# IRepReportOnDrawingInt.OnPolarSystemCurve

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnPolarSystemCurve for DrawingEvents

Specifies the user command that DIAdem REPORT executes when plotting a curve in a polar axis system. The user command receives two parameters. The first parameter corresponds to a PolarCurveDrawingContext object and provides information about the polar axis system and the worksheet in which DIAdem is plotting the curve. The second parameter corresponds to a PolarCurve object and provides information about the curve DIAdem is plotting. This curve is a temporary copy of the curve defined in the axis system. You can change this temporary curve any way you like. After plotting this curve, you can no longer access the temporary PolarCurve object. DIAdem REPORT saves this property with the layout. The user command is only executed if you use the Enable for CurveExpansionSettings property to enable the expansion mode.

## Signature

```python
obj.OnPolarSystemCurve
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnPolarSystemCurve_IRepReportOnDrawingInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
