---
title: "IRepD2AxisDropContextInt.CurveIndex"
description: "Specifies the index of the curve in a 2D axis system onto which you dragged and dropped an object."
---

# IRepD2AxisDropContextInt.CurveIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CurveIndex for D2AxisSystemDropContext

Specifies the index of the curve in a 2D axis system onto which you dragged and dropped an object.

## Signature

```python
obj.CurveIndex
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
dd.AddUserCommandToEvent("dd.Report.Events.OnDrop2DAxisSystem", " MyOnDrop2DAxisSystemEvent")

def MyOnDrop2DAxisSystemEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + "\r\n" + oMyDropElement.Name
    Msgbox(sOutput)
    oMyAxis = Context.AxisSystem
    if Context.CurveIndex>0:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyAxis.Name + "\r\n" + oMyAxis.Curves2D.Item(Context.CurveIndex).Name)
    else:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyAxis.Name)
    Context.DoProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CurveIndex_IRepD2AxisDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
