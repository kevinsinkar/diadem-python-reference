---
title: "ITDMDataStoreConditions.Renumber"
description: "Renews the numbering of search condition names in the search input area of a data store. For example, if you delete the search condition named C2 , the Renumber"
---

# ITDMDataStoreConditions.Renumber

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Renumber for Conditions <DataStore>

Renews the numbering of search condition names in the search input area of a data store. For example, if you delete the search condition named C2 , the Renumber method renews the order of the names.

## Signature

```python
obj.Renumber()
```

## Python example

```python
oMyQueryForm = dd.Navigator.Display.CurrDataStore.QueryForm
oMyQueryForm.Conditions.Add("Measurement","name","=","Car*")
oMyQueryForm.Conditions.Add("Measurement","description","=","My Car Data*")
oMyQuery = oMyQueryForm.GetCurrQuery()
oMyQueryForm.SetCurrQuery(oMyQuery)
oMyQueryForm.Search()
oMyQueryForm.Conditions.Remove(1)
oMyQueryForm.Conditions.Renumber()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Renumber_ITDMDataStoreConditions.htm`*
