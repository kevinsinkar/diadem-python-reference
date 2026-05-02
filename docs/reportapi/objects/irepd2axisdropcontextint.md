---
title: "IRepD2AxisDropContextInt"
description: "The D2AxisSystemDropContext object provides information about the comment onto which you dragged and dropped an object. Do not set the DoProceed property to TRU"
---

# IRepD2AxisDropContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: D2AxisSystemDropContext

The D2AxisSystemDropContext object provides information about the comment onto which you dragged and dropped an object. Do not set the DoProceed property to TRUE if you change the number of curves in the associated event or if you execute similar operations.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisdropcontextint-axissystem/">AxisSystem</a> | <a href="../../properties/irepd2axisdropcontextint-curveindex/">CurveIndex</a> | <a href="../../properties/irepd2axisdropcontextint-doproceed/">DoProceed</a> | <a href="../../properties/irepd2axisdropcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
