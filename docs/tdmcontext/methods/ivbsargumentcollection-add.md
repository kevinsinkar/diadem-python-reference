---
title: "IVbsArgumentCollection.Add"
description: "Adds an element to the Arguments <SystemLink> collection. You cannot edit this argument interactively when defining arguments. However, you can, for example, us"
---

# IVbsArgumentCollection.Add

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: Add for Arguments <SystemLink>

Adds an element to the Arguments <SystemLink> collection. You cannot edit this argument interactively when defining arguments. However, you can, for example, use the argument to exchange values between the procedures.

## Signature

```python
return_value = obj.Add(Name, Value, Type, Description)
```

## Python example

```python
def On_Initialize(oContext):
    oContext.DynamicArguments.Add("AdditionalArgument","StringValue",2,"This is an example for arguments")

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

*Source: `TDMcontext/methods/TDMContext_method_Add_IVbsArgumentCollection.htm`*
