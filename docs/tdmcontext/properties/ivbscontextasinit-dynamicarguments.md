---
title: "IVbsContextASInit.DynamicArguments"
description: "Returns a DynamicArguments for ContextInitialize <Analysis Automation> property. You can add DynamicArguments to the On_Initialize method and read them out in t"
---

# IVbsContextASInit.DynamicArguments

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: DynamicArguments for ContextInitialize <Analysis Automation>

Returns a DynamicArguments for ContextInitialize <Analysis Automation> property. You can add DynamicArguments to the On_Initialize method and read them out in the methods On_Run_AnalysisProcedure and On_Finalize .

## Signature

```python
return_value = obj.DynamicArguments
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

*Source: `TDMcontext/properties/TDMContext_property_DynamicArguments_IVbsContextASInit.htm`*
