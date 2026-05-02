---
title: "IRepReportEventsInt.OnLayoutLoaded"
description: "Is triggered in DIAdem REPORT when you load a layout. The event starts the user command that you have assigned to the property Report.Events. OnLayoutLoaded . T"
---

# IRepReportEventsInt.OnLayoutLoaded

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnLayoutLoaded for Events

Is triggered in DIAdem REPORT when you load a layout. The event starts the user command that you have assigned to the property Report.Events. OnLayoutLoaded . The user command has no parameters. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnLayoutLoaded
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
dd.AddUserCommandToEvent("dd.Report.Events.OnLayoutLoaded", "MyOnLayoutLoadedEvent")

def MyOnLayoutLoadedEvent():
    if dd.Report.ActiveSheet.Objects.Exists("MyLoadText"):
        dd.Report.ActiveSheet.Objects("MyLoadText").Text  = "Layout loaded at @@CurrTime@@"
    else:
        oMyText = dd.Report.ActiveSheet.Objects.Add(eReportObjectText,"MyLoadText")
        oMyText.Text = "Layout loaded at @@CurrTime@@"
    dd.MsgBox("Layout loaded")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnLayoutLoaded_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
