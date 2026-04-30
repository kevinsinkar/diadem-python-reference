---
title: "IDataFinderQuery.ReturnType"
description: "Specifies the return type of the search results in a search without the user interface in a DataFinder."
---

# IDataFinderQuery.ReturnType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ReturnType for Query <DataFinder>

Specifies the return type of the search results in a search without the user interface in a DataFinder.

## Signature

```python
obj.ReturnType
```

## Python example

```python
dd.Data.Root.Clear()
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchFile
oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Weather.tdm")
oMyDataFinder.SearchElements(oMyQuery, 200)
oMyResults = oMyDataFinder.ResultsElements
dd.Navigator.LoadData(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ReturnType_IDataFinderQuery.htm`*
