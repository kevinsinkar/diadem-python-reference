---
title: "IVbsArgumentCollection.GetOrCreate"
description: "Returns an element of the Arguments <SystemLink> collection or creates an element if there is no argument."
---

# IVbsArgumentCollection.GetOrCreate

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: GetOrCreate for Arguments <SystemLink>

Returns an element of the Arguments <SystemLink> collection or creates an element if there is no argument.

## Signature

```python
return_value = obj.GetOrCreate(Name, type, defValue)
```

## Python example

```python
def On_Initialize(oContext):
    oContext.DynamicArguments.GetOrCreate("AdditionalArgument","StringValue",2,"This is an example for arguments")

def On_Run_AnalysisProcedure(oContext):
    sExchangeArg = oContext.DynamicArguments.Item("AdditionalArgument").Value
    oContext.LogResult("Value of Argument: " + sExchangeArg)
# Enter your analysis commands
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_GetOrCreate_IVbsArgumentCollection.htm`*
