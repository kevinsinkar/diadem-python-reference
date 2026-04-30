---
title: "IRepCommentTextInt"
description: "The CommentElement object provides the text and frame properties of a comment in DIAdem REPORT."
---

# IRepCommentTextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CommentElement

The CommentElement object provides the text and frame properties of a comment in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcommenttextint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepcommenttextint-borderline/">BorderLine</a> | <a href="../../properties/irepcommenttextint-font/">Font</a> | <a href="../../properties/irepcommenttextint-text/">Text</a> | <a href="../../properties/irepcommenttextint-textalignmenthorizontal/">TextAlignmentHorizontal</a> | <a href="../../properties/irepcommenttextint-textalignmentvertical/">TextAlignmentVertical</a> | <a href="../../properties/irepcommenttextint-textmargin/">TextMargin</a> | <a href="../../properties/irepcommenttextint-textrotation/">TextRotation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcommentint/">Comment</a>.<a href="../../properties/irepcommentint-comment/">Comment</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCommentTextInt.htm`*
