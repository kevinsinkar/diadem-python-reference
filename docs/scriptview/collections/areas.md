---
title: "Areas"
description: "The Areas object provides a collection of all the areas in DIAdem VIEW. Use the areas collection to delete areas. To create new areas, split an existing Area Ob"
---

# Areas

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Areas

The Areas object provides a collection of all the areas in DIAdem VIEW. Use the areas collection to delete areas. To create new areas, split an existing Area Object .

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.Name = "MySheet"
oMyArea = oMySheet.ActiveArea
oMyNewArea = oMyArea.SplitRight("NewArea", 0.5)
oMyNewArea.Active = True
oMyNewArea.DisplayObjType = "CurveChart2D"
oMyChart = oMyNewArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoareaobjectscontint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoareaobjectscontint-copy/">Copy</a> | <a href="../../methods/itoareaobjectscontint-exists/">Exists</a> | <a href="../../methods/itoareaobjectscontint-item/">Item</a> | <a href="../../methods/itoareaobjectscontint-move/">Move</a> | <a href="../../methods/itoareaobjectscontint-remove/">Remove</a> | <a href="../../methods/itoareaobjectscontint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itosheetint/">Sheet</a>.<a href="../../properties/itosheetint-areas/">Areas</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToAreaObjectsContInt.htm`*
