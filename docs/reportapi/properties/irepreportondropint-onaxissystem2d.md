---
title: "IRepReportOnDropInt.OnAxisSystem2D"
description: "Specifies the user command that DIAdem REPORT executes when you drag and drop an element onto a 2D axis system. The user command receives two parameters. The fi"
---

# IRepReportOnDropInt.OnAxisSystem2D

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnAxisSystem2D for DropEvents

Specifies the user command that DIAdem REPORT executes when you drag and drop an element onto a 2D axis system. The user command receives two parameters. The first parameter corresponds to a D2AxisSystemDropContext object and provides information about the 2D axis system onto which you dragged and dropped an object. The second parameter corresponds to a DropInformation object and provides information about the object which you dragged and dropped onto another object. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnAxisSystem2D
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
dd.Report.Events.Drop.OnAxisSystem2D = " MyOnDrop2DAxisSystemEvent"

def MyOnDrop2DAxisSystemEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + VBCrLf + oMyDropElement.Name
    Msgbox(sOutput)
    oMyAxis = Context.AxisSystem
    if Context.CurveIndex>0:
        dd.MsgBox(Context.Sheet.Name + VBCrLf + oMyAxis.Name + VBCrLf + oMyAxis.Curves2D.Item(Context.CurveIndex).Name)
    else:
        dd.MsgBox(Context.Sheet.Name + VBCrLf + oMyAxis.Name)
    Context.DoProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnAxisSystem2D_IRepReportOnDropInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
