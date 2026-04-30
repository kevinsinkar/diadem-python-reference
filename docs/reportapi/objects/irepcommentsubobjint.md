---
title: "IRepCommentSubObjInt"
description: "The CommentSubObj object provides information about a subobject of a comment in DIAdem REPORT when DIAdem calls the event assigned to the OnComment for ToolTipE"
---

# IRepCommentSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CommentSubObj

The CommentSubObj object provides information about a subobject of a comment in DIAdem REPORT when DIAdem calls the event assigned to the OnComment for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnComment = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + VBCrLf + "Sub object" + VBCrLf + "Name: " + oSubObject.Name + VBCrLf + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + VBCrLf + "X position: " + Context.Position.X + VBCrLf + "Y position: " + Context.Position.Y
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcommentsubobjint-name/">Name</a> | <a href="../../properties/irepcommentsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptooltipcommentcontextint/">ToolTipCommentContext</a>.<a href="../../properties/ireptooltipcommentcontextint-subobject/">SubObject</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCommentSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
