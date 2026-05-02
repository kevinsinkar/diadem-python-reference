---
title: "IRepReportOnDropInt.OnPolarSystem"
description: "Is triggered in DIAdem REPORT when you drag and drop an element onto a polar axis system. The event starts the user command that you assigned to the OnPolarSyst"
---

# IRepReportOnDropInt.OnPolarSystem

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnPolarSystem for DropEvents

Is triggered in DIAdem REPORT when you drag and drop an element onto a polar axis system. The event starts the user command that you assigned to the OnPolarSystem for DropEvents property. The user command receives two parameters. The first parameter corresponds to a PolarSystemDropContext object and provides information about the worksheet onto which you dragged and dropped an object. The second parameter corresponds to a DropInformation object and provides information about the object which you dragged and dropped onto another object. DIAdem REPORT saves this property with the layout. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnPolarSystem
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
AddUserCommandToEvent("dd.Report.Events.OnDropPolarSystem", "MyOnDropPolarSystemEvent")

def MyOnDropPolarSystemEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + "\r\n" + oMyDropElement.Name
    Msgbox(sOutput)
    oMyAxis = Context.PolarSystem
    if Context.CurveIndex>0:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyAxis.Name + "\r\n" + oMyAxis.CurvesPolar.Item(Context.CurveIndex).Name)
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

*Source: `ReportApi/events/Report_event_OnPolarSystem_IRepReportOnDropInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
