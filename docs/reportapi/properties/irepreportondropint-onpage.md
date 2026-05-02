---
title: "IRepReportOnDropInt.OnPage"
description: "Specifies the user command that DIAdem REPORT executes when you drag and drop an element onto a worksheet. The user command receives two parameters. The first p"
---

# IRepReportOnDropInt.OnPage

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnPage for DropEvents

Specifies the user command that DIAdem REPORT executes when you drag and drop an element onto a worksheet. The user command receives two parameters. The first parameter corresponds to a PageDropContext object and provides information about the worksheet onto which you dragged and dropped an object. The second parameter corresponds to a DropInformation object and provides information about the object which you dragged and dropped onto another object. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnPage
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.Events.Drop.OnPage = "MyOnDropPageEvent"

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

*Source: `ReportApi/properties/Report_property_OnPage_IRepReportOnDropInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
