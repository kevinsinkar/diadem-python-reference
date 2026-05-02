---
title: "IRepDropPositionInt"
description: "The DropPosition object provides information about the position onto which you dragged and dropped an object."
---

# IRepDropPositionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: DropPosition

The DropPosition object provides information about the position onto which you dragged and dropped an object.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepdroppositionint-x/">X</a> | <a href="../../properties/irepdroppositionint-y/">Y</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppagedropcontextint/">PageDropContext</a>.<a href="../../properties/ireppagedropcontextint-position/">Position</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepDropPositionInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
