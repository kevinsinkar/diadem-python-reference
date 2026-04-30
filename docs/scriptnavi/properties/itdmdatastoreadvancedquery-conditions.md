---
title: "ITDMDataStoreAdvancedQuery.Conditions"
description: "Specifies the search parameters for a search without the interface in a data store."
---

# ITDMDataStoreAdvancedQuery.Conditions

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Conditions for AdvancedQuery <DataStore>

Specifies the search parameters for a search without the interface in a data store.

## Signature

```python
return_value = obj.Conditions
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Conditions_ITDMDataStoreAdvancedQuery.htm`*
