---
title: "IVbsArgumentCollection.Count"
description: "Returns the number of arguments."
---

# IVbsArgumentCollection.Count

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: Count for Arguments <SystemLink>

Returns the number of arguments.

## Signature

```python
iCount = Object.Count
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    oArguments = oContext.Procedure.Arguments
    for iCount in range( 1, oArguments.Count+1):
        sParamName  = oArguments(iCount).Name
        vParamValue = oArguments(iCount).Value
        oContext.LogResult(sParamName + ": " + vParamValue)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_Count_IVbsArgumentCollection.htm`*
