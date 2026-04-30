---
title: "IRepD3AxisDropContextInt.DoProceed"
description: "Specifies whether DIAdem transfers the D3AxisSystemDropContext object to subsequent events. If the value is TRUE , DIAdem also transfers the D3AxisSystemDropCon"
---

# IRepD3AxisDropContextInt.DoProceed

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DoProceed for D3AxisSystemDropContext

Specifies whether DIAdem transfers the D3AxisSystemDropContext object to subsequent events. If the value is TRUE , DIAdem also transfers the D3AxisSystemDropContext object to the following events. Do not set the DoProceed property to TRUE if you change the number of curves in the associated event or if you execute similar operations.

## Signature

```python
obj.DoProceed
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
AddUserCommandToEvent("dd.Report.Events.OnDrop3DAxisSystem", "MyOnDrop3DAxisSystemEvent")

def MyOnDrop3DAxisSystemEvent(Context,DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + VBCrLf + oMyDropElement.Name
    Msgbox(sOutput)
    oMyAxis = Context.AxisSystem
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

*Source: `ReportApi/properties/Report_property_DoProceed_IRepD3AxisDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
