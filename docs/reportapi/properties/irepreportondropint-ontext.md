---
title: "IRepReportOnDropInt.OnText"
description: "Specifies the user command that DIAdem REPORT executes when you drag and drop an element onto a text. The user command receives two parameters. The first parame"
---

# IRepReportOnDropInt.OnText

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnText for DropEvents

Specifies the user command that DIAdem REPORT executes when you drag and drop an element onto a text. The user command receives two parameters. The first parameter corresponds to a TextDropContext object and provides information about the text onto which you dragged and dropped an object. The second parameter corresponds to a DropInformation object and provides information about the object which you dragged and dropped onto another object. DIAdem REPORT saves this property with the layout.

## Signature

```python
obj.OnText
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
dd.Report.Events.Drop.OnText = "MyOnDropTextEvent"

def MyOnDropTextEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + VBCrLf + oMyDropElement.Name
    dd.MsgBox(sOutput)
    oMyText = Context.Text
    dd.MsgBox(Context.Sheet.Name + VBCrLf + oMyText.Name + VBCrLf + oMyText.Text)
    Context.DoProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnText_IRepReportOnDropInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
