---
title: "VIEW"
description: "The View object accesses the subobjects in DIAdem VIEW. Use the View object to load and to save layouts. The View object is available as a global object in scri"
---

# VIEW

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: View

The View object accesses the subobjects in DIAdem VIEW. Use the View object to load and to save layouts. The View object is available as a global object in scripts and in dialog boxes.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Do assign the name View to any of the objects and variables you create because that overwrites the View object.</td></tr></table>
</div>

## Python example

```python
oMySheet = dd.View.ActiveSheet
print(oMySheet.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/view-activesheet/">ActiveSheet</a> | <a href="../../properties/view-autorefresh/">AutoRefresh</a> | <a href="../../properties/view-coordinatewnd/">CoordinateWnd</a> | <a href="../../properties/view-currsheet/">CurrSheet</a> | <a href="../../properties/view-events/">Events</a> | <a href="../../properties/view-filename/">FileName</a> | <a href="../../properties/view-fullpath/">FullPath</a> | <a href="../../properties/view-layoutmodified/">LayoutModified</a> | <a href="../../properties/view-settings/">Settings</a> | <a href="../../properties/view-sheets/">Sheets</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/view-appendlayout/">AppendLayout</a> | <a href="../../methods/view-loadlayout/">LoadLayout</a> | <a href="../../methods/view-newlayout/">NewLayout</a> | <a href="../../methods/view-refresh/">Refresh</a> | <a href="../../methods/view-savelayout/">SaveLayout</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_VIEW.htm`*
