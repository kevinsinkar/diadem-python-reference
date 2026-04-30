---
title: "IRepReportOnDropInt"
description: "The DropEvents object provides the events when dragging and dropping onto a REPORT object."
---

# IRepReportOnDropInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: DropEvents

The DropEvents object provides the events when dragging and dropping onto a REPORT object.

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
<p><a href="../../properties/irepreportondropint-onaxissystem2d/">OnAxisSystem2D</a> | <a href="../../properties/irepreportondropint-onaxissystem3d/">OnAxisSystem3D</a> | <a href="../../properties/irepreportondropint-oncomment/">OnComment</a> | <a href="../../properties/irepreportondropint-onpage/">OnPage</a> | <a href="../../properties/irepreportondropint-onpolarsystem/">OnPolarSystem</a> | <a href="../../properties/irepreportondropint-ontable2d/">OnTable2D</a> | <a href="../../properties/irepreportondropint-ontable3d/">OnTable3D</a> | <a href="../../properties/irepreportondropint-ontext/">OnText</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepreporteventsint/">Events</a>.<a href="../../properties/irepreporteventsint-drop/">Drop</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepReportOnDropInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
