---
title: "FreeElementList"
description: "Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of elements. Use the FreeElementList collection to access data store elements. "
---

# FreeElementList

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: FreeElementList <DataStore>

Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of elements. Use the FreeElementList collection to access data store elements. You can add elements to the collection or remove elements from the collection. The data in DIAdem NAVIGATOR remains unchanged. Each element of the ElementList collection is an Element <DataStore> .

## Python example

```python
dd.Data.Root.Clear()
oMyStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyQuery = oMyStore.CreateQuery
oMyConditions = oMyQuery.Conditions
oMyConditions.Add("measurement","name","=","TL2700_1")
oMyStore.SearchElements(oMyQuery)
oMyResults = oMyStore.ResultsElements
oMyElementList = oMyStore.CreateElementList()
oMyElementList.AddElementList(oMyResults)
for Element in oMyElementList:
    Output = Output + Element.Name + "\r\n"
dd.MsgBoxDisp(Output)
dd.Navigator.LoadData(oMyElementList)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmfreestoreelementlist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmfreestoreelementlist-add/">Add</a> | <a href="../../methods/itdmfreestoreelementlist-addelementlist/">AddElementList</a> | <a href="../../methods/itdmfreestoreelementlist-exists/">Exists</a> | <a href="../../methods/itdmfreestoreelementlist-item/">Item</a> | <a href="../../methods/itdmfreestoreelementlist-remove/">Remove</a> | <a href="../../methods/itdmfreestoreelementlist-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-createelementlist/">CreateElementList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMFreeStoreElementList.htm`*
