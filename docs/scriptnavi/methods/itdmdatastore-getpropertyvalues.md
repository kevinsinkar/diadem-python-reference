---
title: "ITDMDataStore.GetPropertyValues"
description: "Returns the values of properties or the minimum and maximum values of a property, in a data store. You can also assign a search request as a parameter to the Ge"
---

# ITDMDataStore.GetPropertyValues

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetPropertyValues for DataStore

Returns the values of properties or the minimum and maximum values of a property, in a data store. You can also assign a search request as a parameter to the GetPropertyValues method.

## Signature

```python
vGetPropertyValues = Object.GetPropertyValues(EntityName, PropertyName, Query, Aggregation, OdsConform)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAggregateDistinct` | 1 | Returns a list with the values of the PropertyName property. |
| `eAggregateMinMax` | 2 | Returns the value range of the PropertyName property. |

## Python example

```python
store = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
values = store.GetPropertyValues("TestRun", "name", "measurements.name=Q*", dd.eAggregateDistinct, False)
print(values)
```

```python
store = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
query = store.CreateQuery()
query.Conditions.Add("Measurement", "name", "=", "Q*")
query.Conditions.Add("TestRun", "name", "=", "TR_M17_QT_32*")
query.Conditions.Add("MeaQuantity", "minimum", ">", 0)
query.ReturnType = "MeaQuantity"
values = store.GetPropertyValues("", "minimum", query, dd.eAggregateMinMax, False)
if len(values) != 0:
    print("Minimum:", values[0])
    print("Maximum:", values[1])
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetPropertyValues_ITDMDataStore.htm`*
