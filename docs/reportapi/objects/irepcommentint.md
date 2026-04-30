---
title: "IRepCommentInt"
description: "The Comment object provides a comment in DIAdem REPORT."
---

# IRepCommentInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Comment

The Comment object provides a comment in DIAdem REPORT.

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
<p><a href="../../properties/irepcommentint-arrow/">Arrow</a> | <a href="../../properties/irepcommentint-comment/">Comment</a> | <a href="../../properties/irepcommentint-index/">Index</a> | <a href="../../properties/irepcommentint-isselected/">IsSelected</a> | <a href="../../properties/irepcommentint-name/">Name</a> | <a href="../../properties/irepcommentint-objecttype/">ObjectType</a> | <a href="../../properties/irepcommentint-position/">Position</a> | <a href="../../properties/irepcommentint-selectedelements/">SelectedElements</a> | <a href="../../properties/irepcommentint-tagstored/">TagStored</a> | <a href="../../properties/irepcommentint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepcommentint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepcommentint-select/">Select</a> | <a href="../../methods/irepcommentint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcommentdropcontextint/">CommentDropContext</a>.<a href="../../properties/irepcommentdropcontextint-comment/">Comment</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../ireptooltipcommentcontextint/">ToolTipCommentContext</a>.<a href="../../properties/ireptooltipcommentcontextint-comment/">Comment</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCommentInt.htm`*
