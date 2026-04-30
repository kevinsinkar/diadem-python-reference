---
title: "IRepDropPositionInt.X"
description: "Specifies the x-position in a worksheet onto which you dragged and dropped an object in DIAdem REPORT."
---

# IRepDropPositionInt.X

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: X for DropPosition

Specifies the x-position in a worksheet onto which you dragged and dropped an object in DIAdem REPORT.

## Signature

```python
obj.X
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
AddUserCommandToEvent("dd.Report.Events.OnDropPage", "MyOnDropPageEvent")

def MyOnDropPageEvent(Context, DropContext):
    sOutput = "Names of dropped elements:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + VBCrLf + oMyDropElement.Name
    Msgbox(sOutput)
    dd.MsgBox(Context.Sheet.Name + VBCrLf + Context.Position.X + VBCrLf + Context.Position.Y)
    Context.DoProceed = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_X_IRepDropPositionInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
