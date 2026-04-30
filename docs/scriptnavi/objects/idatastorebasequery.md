---
title: "IDataStoreBaseQuery"
description: "The Query object provides a search object in a data store. You can use this search object for a Search with the interface of DIAdem NAVIGATOR and for a Search w"
---

# IDataStoreBaseQuery

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Query <DataStore>

The Query object provides a search object in a data store. You can use this search object for a Search with the interface of DIAdem NAVIGATOR and for a Search without the interface . You can run a Quick search and an Advanced search with this search object. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. The Query object corresponds to one of the following objects: AdvancedQuery (ITDMDataStoreAdvancedQuery) Advanced Search TextQuery (IDataStoreTextQuery) Quick Search

## Python example

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
oMyStore = dd.Navigator.Display.CurrDataStore
oMyQueryForm = oMyStore.QueryForm
oMyQueryForm.Conditions.RemoveAll()
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add("Test","Name","=","ETC")
oMyConditions.Add("Measurement","Name","=","DL")
oMyConditions.Logic = "C1 and C2"
oMyQuery = oMyQueryForm.GetCurrQuery()
if (oMyQuery.IsKindOf(dd.eDataStoreQuery)) :
    for Condition in oMyQuery.Conditions:
        dd.MsgBoxDisp("Property: " + Condition.Property + "\r\n" + "Value: " + Condition.Value)
oMyQueryForm.Search()
dd.Navigator.LoadData(oMyStore.ResultsList.ResultsElements,"Load")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatastorebasequery-returntype/">ReturnType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatastorebasequery-isempty/">IsEmpty</a> | <a href="../../methods/idatastorebasequery-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-createquery/">CreateQuery</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-loadquery/">LoadQuery</a> | <a href="../inavidatastorequeryform/">QueryForm &lt;DataStore&gt;</a>.<a href="../../methods/inavidatastorequeryform-getcurrquery/">GetCurrQuery</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataStoreBaseQuery.htm`*
