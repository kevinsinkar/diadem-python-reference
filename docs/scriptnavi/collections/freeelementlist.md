---
title: "FreeElementList"
description: "Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of elements. Use the FreeElementList collection to access channels, channel gro"
---

# FreeElementList

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: FreeElementList <DataFinder>

Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of elements. Use the FreeElementList collection to access channels, channel groups, or the root of a DataFinder. You can add elements to the collection or remove elements from the collection. The data in DIAdem NAVIGATOR remains unchanged. Each element of the ElementList collection is an Element <DataFinder> .

## Python example

```python
dd.Data.Root.Clear()
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList = oMyDataFinder.CreateElementList()
oMyElementList.AddElementlist(oMyResults)
for Element in oMyElementList:
    Output = Output + Element.Name + "\r\n"
dd.MsgBoxDisp(Output)
dd.Navigator.LoadData(oMyElementList)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmfreedatafinderelementlist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmfreedatafinderelementlist-add/">Add</a> | <a href="../../methods/itdmfreedatafinderelementlist-addelementlist/">AddElementList</a> | <a href="../../methods/itdmfreedatafinderelementlist-exists/">Exists</a> | <a href="../../methods/itdmfreedatafinderelementlist-item/">Item</a> | <a href="../../methods/itdmfreedatafinderelementlist-remove/">Remove</a> | <a href="../../methods/itdmfreedatafinderelementlist-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmdatafinder/">DataFinder</a>.<a href="../../methods/itdmdatafinder-createelementlist/">CreateElementList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMFreeDataFinderElementList.htm`*
