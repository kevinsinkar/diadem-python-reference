---
title: "IRepPageDropContextInt.DoProceed"
description: "Specifies whether DIAdem transfers the PageDropContext object to subsequent events. If the value is TRUE , DIAdem also transfers the PageDropContext object to t"
---

# IRepPageDropContextInt.DoProceed

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DoProceed for PageDropContext

Specifies whether DIAdem transfers the PageDropContext object to subsequent events. If the value is TRUE , DIAdem also transfers the PageDropContext object to the following events. Do not set the DoProceed property to TRUE if you delete the page object in the associated event or if you execute similar operations.

## Signature

```python
obj.DoProceed
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

*Source: `ReportApi/properties/Report_property_DoProceed_IRepPageDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
