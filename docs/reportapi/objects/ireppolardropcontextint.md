---
title: "IRepPolarDropContextInt"
description: "The PolarSystemDropContext object provides information about the polar axis system onto which you dragged and dropped an object. Do not set the DoProceed proper"
---

# IRepPolarDropContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarSystemDropContext

The PolarSystemDropContext object provides information about the polar axis system onto which you dragged and dropped an object. Do not set the DoProceed property to TRUE if you change the number of curves in the associated event or if you execute similar operations.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.Report.Events.OnDropPolarSystem", "MyOnDropPolarSystemEvent")

def MyOnDropPolarSystemEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + VBCrLf + oMyDropElement.Name
    Msgbox(sOutput)
    oMyAxis = Context.PolarSystem
    if Context.CurveIndex>0:
        dd.MsgBox(Context.Sheet.Name + VBCrLf + oMyAxis.Name + VBCrLf + oMyAxis.CurvesPolar.Item(Context.CurveIndex).Name)
    else:
        dd.MsgBox(Context.Sheet.Name + VBCrLf + oMyAxis.Name)
    Context.DoProceed = TRUE
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolardropcontextint-curveindex/">CurveIndex</a> | <a href="../../properties/ireppolardropcontextint-doproceed/">DoProceed</a> | <a href="../../properties/ireppolardropcontextint-polarsystem/">PolarSystem</a> | <a href="../../properties/ireppolardropcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
