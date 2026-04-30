---
title: "IRepPageDropContextInt"
description: "The PageDropContext object provides information about the page onto which you dragged and dropped an object. Do not set the DoProceed property to TRUE if you ch"
---

# IRepPageDropContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PageDropContext

The PageDropContext object provides information about the page onto which you dragged and dropped an object. Do not set the DoProceed property to TRUE if you change the number of pages in the associated event or if you execute similar operations.

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
    Context.DoProceed = TRUE
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppagedropcontextint-doproceed/">DoProceed</a> | <a href="../../properties/ireppagedropcontextint-position/">Position</a> | <a href="../../properties/ireppagedropcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPageDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
