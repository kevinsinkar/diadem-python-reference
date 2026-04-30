---
title: "IRepCommentDropContextInt.Sheet"
description: "Specifies the worksheet that contains the comment onto which you dragged and dropped an object."
---

# IRepCommentDropContextInt.Sheet

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sheet for CommentDropContext

Specifies the worksheet that contains the comment onto which you dragged and dropped an object.

## Signature

```python
return_value = obj.Sheet
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
AddUserCommandToEvent("dd.Report.Events.OnDropComment", "MyOnDropCommentEvent")

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

*Source: `ReportApi/properties/Report_property_Sheet_IRepCommentDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
