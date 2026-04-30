---
title: "Sheets"
description: "The Sheets object provides a collection of all Worksheets in DIAdem VIEW. Use the Sheets object to delete worksheets or to add new worksheets in the layout."
---

# Sheets

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Sheets

The Sheets object provides a collection of all Worksheets in DIAdem VIEW. Use the Sheets object to delete worksheets or to add new worksheets in the layout.

## Python example

```python
for oMySheet in dd.View.Sheets:
    dd.MsgBoxDisp(oMySheet.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itosheetcontint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itosheetcontint-add/">Add</a> | <a href="../../methods/itosheetcontint-exists/">Exists</a> | <a href="../../methods/itosheetcontint-item/">Item</a> | <a href="../../methods/itosheetcontint-printall/">PrintAll</a> | <a href="../../methods/itosheetcontint-remove/">Remove</a> | <a href="../../methods/itosheetcontint-removeall/">RemoveAll</a> | <a href="../../methods/itosheetcontint-showprintdlg/">ShowPrintDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/view/">View</a>.<a href="../../properties/view-sheets/">Sheets</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSheetContInt.htm`*
