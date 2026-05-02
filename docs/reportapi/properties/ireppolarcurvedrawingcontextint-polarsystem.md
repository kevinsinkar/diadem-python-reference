---
title: "IRepPolarCurveDrawingContextInt.PolarSystem"
description: "Specifies the polar axis system of the curve DIAdem REPORT is plotting."
---

# IRepPolarCurveDrawingContextInt.PolarSystem

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PolarSystem for PolarCurveDrawingContext

Specifies the polar axis system of the curve DIAdem REPORT is plotting.

## Signature

```python
return_value = obj.PolarSystem
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
AddUserCommandToEvent("dd.Report.Events.OnDrawingPolarSystemCurve", "MyOnPolarCurveDrawEvent")

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

dd.MsgBox("Sheet: " + Context.Sheet.Name + "\r\n" + "Axis system: " + oMyAxis.Name + "Curve name: " + oMyCurve.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PolarSystem_IRepPolarCurveDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
