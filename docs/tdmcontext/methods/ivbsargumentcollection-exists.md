---
title: "IVbsArgumentCollection.Exists"
description: "Checks whether an argument with a specific name exists."
---

# IVbsArgumentCollection.Exists

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: Exists for Arguments <SystemLink>

Checks whether an argument with a specific name exists.

## Signature

```python
bExists = Object.Exists(Name)
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

*Source: `TDMcontext/methods/TDMContext_method_Exists_IVbsArgumentCollection.htm`*
