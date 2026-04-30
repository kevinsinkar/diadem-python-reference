---
title: "IVbsArgumentCollection.Item"
description: "Returns an individual element of the Arguments <SystemLink> collection."
---

# IVbsArgumentCollection.Item

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Item for Arguments <SystemLink>

Returns an individual element of the Arguments <SystemLink> collection.

## Signature

```python
return_value = obj.Item(nameOrIndex)
```

## Python example

```python
def On_Initialize(oContext):
    if oContext.Procedure.Arguments.Exists("ResultsPath") :
        ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
        oContext.LogResult("Results path: " + ResultsPath)
    else:
        oContext.LogError("Results path missing")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_Item_IVbsArgumentCollection.htm`*
