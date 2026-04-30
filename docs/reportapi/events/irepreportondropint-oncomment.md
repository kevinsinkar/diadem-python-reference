---
title: "IRepReportOnDropInt.OnComment"
description: "Is triggered in DIAdem REPORT when you drag and drop an element onto a comment. The event starts the user command that you assigned to the OnComment for DropEve"
---

# IRepReportOnDropInt.OnComment

!!! abstract "Event &middot; `ReportApi.chm`"
    Event: OnComment for DropEvents

Is triggered in DIAdem REPORT when you drag and drop an element onto a comment. The event starts the user command that you assigned to the OnComment for DropEvents property. The first parameter corresponds to a CommentDropContext object and provides information about the comment onto which you dragged and dropped an object. The second parameter corresponds to a DropInformation object and provides information about the object which you dragged and dropped onto another object. DIAdem REPORT saves this property with the layout. Refer to Working with Events in DIAdem for further information on events in DIAdem.

## Signature

```python
obj.OnComment
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
AddUserCommandToEvent("dd.Report.Events.Drop.OnComment", "MyOnDropCommentEvent")

def MyOnDropCommentEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + VBCrLf + oMyDropElement.Name
    Msgbox(sOutput)
    oMyComment = Context.Comment
    dd.MsgBox(Context.Sheet.Name + VBCrLf + oMyComment.Name)
    Context.DoProceed = TRUE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/events/Report_event_OnComment_IRepReportOnDropInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
