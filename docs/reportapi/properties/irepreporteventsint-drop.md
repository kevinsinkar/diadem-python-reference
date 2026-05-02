---
title: "IRepReportEventsInt.Drop"
description: "Returns the object in DIAdem REPORT that provides the events when you drag and drop onto a REPORT object."
---

# IRepReportEventsInt.Drop

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Drop for Events

Returns the object in DIAdem REPORT that provides the events when you drag and drop onto a REPORT object.

## Signature

```python
return_value = obj.Drop
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
dd.AddUserCommandToEvent("dd.Report.Events.OnDropPage", "MyOnDropPageEvent")

def MyOnDropPageEvent(Context, DropContext):
    sOutput = "Names of dropped elements:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + "\r\n" + oMyDropElement.Name
    Msgbox(sOutput)
    dd.MsgBox(Context.Sheet.Name + "\r\n" + Context.Position.X + "\r\n" + Context.Position.Y)
    Context.DoProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Drop_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
