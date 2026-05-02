---
title: "IRepReportEventsInt.OnLayoutSaving"
description: "Specifies the user command that DIAdem REPORT executes when saving a layout. The user command has one parameter. The parameter contains the complete layout path"
---

# IRepReportEventsInt.OnLayoutSaving

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnLayoutSaving for Events

Specifies the user command that DIAdem REPORT executes when saving a layout. The user command has one parameter. The parameter contains the complete layout path and the filename.

## Signature

```python
obj.OnLayoutSaving
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
dd.AddUserCommandToEvent("dd.Report.Events.OnLayoutSaving", "MyOnLayoutSavingEvent")

def MyOnLayoutSavingEvent(sLayout):
    if dd.Report.ActiveSheet.Objects.Exists("MyLoadText"):
        dd.Report.ActiveSheet.Objects("MyLoadText").Text  = "Layout name: " + sLayout
    else:
        oMyText = dd.Report.ActiveSheet.Objects.Add(eReportObjectText,"MyLoadText")
        oMyText.Text = "Layout name: " + sLayout
    dd.Report.Refresh()
    dd.MsgBox("Layout name: " + sLayout)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnLayoutSaving_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
