---
title: "ITDMDataFinder.SearchElements"
description: "Makes a search without user interface for elements from the DataFinder. You must transfer the search conditions as a parameter. Use the SearchElements method to"
---

# ITDMDataFinder.SearchElements

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SearchElements for DataFinder

Makes a search without user interface for elements from the DataFinder. You must transfer the search conditions as a parameter. Use the SearchElements method to execute a Quick search and an Advanced search . Use the ResultsElements property to access the search results.

## Signature

```python
obj.SearchElements(Query, [MaxCount])
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.Conditions.Add(dd.eSearchChannel,"name","=","Time")
oMyDataFinder.SearchElements(oMyQuery)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SearchElements_ITDMDataFinder.htm`*
