---
title: "IRepPolarCurveDrawingContextInt.Sheet"
description: "Specifies the worksheet of the curve DIAdem is plotting in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveDrawingContextInt.Sheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sheet for PolarCurveDrawingContext

Specifies the worksheet of the curve DIAdem is plotting in a polar axis system in DIAdem REPORT.

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

dd.MsgBox("Sheet: " + Context.Sheet.Name + VBCrLf + "Axis system: " + oMyAxis.Name + "Curve name: " + oMyCurve.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Sheet_IRepPolarCurveDrawingContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
