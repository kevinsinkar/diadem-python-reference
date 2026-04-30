---
title: "ITDMDataStoreAdvancedQuery.IsKindOf"
description: "Determines in a data store whether you run a quick search or an advanced search."
---

# ITDMDataStoreAdvancedQuery.IsKindOf

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsKindOf for AdvancedQuery <DataStore>

Determines in a data store whether you run a quick search or an advanced search.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAdvancedQuery` | 1 | Advanced search (DataFinder) |
| `eTextQuery` | 2 | Quick search (DataFinder) |
| `eDataStoreQuery` | 4 | Advanced search (DataFinder) |
| `eDataStoreTextQuery` | 8 | Quick search (DataStore) |

## Python example

```python
oMyQuery = dd.Navigator.Display.CurrDataStore.QueryForm.GetCurrQuery()
if (oMyQuery.IsKindOf(dd.eDataStoreTextQuery)) :
    dd.MsgBoxDisp(oMyQuery.Text)
elif (oMyQuery.IsKindOf(dd.eDataStoreQuery)) :
    oMyConditions = oMyQuery.Conditions
    for Condition in oMyConditions:
        dd.MsgBoxDisp (Condition.Property + Condition.Operator + Condition.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsKindOf_ITDMDataStoreAdvancedQuery.htm`*
