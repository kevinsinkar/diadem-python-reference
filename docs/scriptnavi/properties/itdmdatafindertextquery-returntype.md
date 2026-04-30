---
title: "ITDMDataFinderTextQuery.ReturnType"
description: "Specifies the search results type of a search in a data store. The search result of a quick search in a DataFinder is always a file type."
---

# ITDMDataFinderTextQuery.ReturnType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ReturnType for TextQuery <DataFinder>

Specifies the search results type of a search in a data store. The search result of a quick search in a DataFinder is always a file type.

## Signature

```python
obj.ReturnType
```

## Python example

```python
oMyDataFinder = dd.NAVIGATOR.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eTextQuery)
oMyQuery.Text = "SearchValue"
dd.MsgBoxDisp(oMyQuery.ReturnType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ReturnType_ITDMDataFinderTextQuery.htm`*
