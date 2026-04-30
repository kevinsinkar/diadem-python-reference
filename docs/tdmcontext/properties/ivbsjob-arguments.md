---
title: "IVbsJob.Arguments"
description: "Returns the Arguments <SystemLink> collection in the methods of Analysis Automation. This collection contains the list of transferred parameters. You can extend"
---

# IVbsJob.Arguments

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Arguments for Procedure <Analysis Automation>

Returns the Arguments <SystemLink> collection in the methods of Analysis Automation. This collection contains the list of transferred parameters. You can extend the Arguments <SystemLink> collection with the DynamicArguments property in the On_Initialize method in order to extend further arguments which you read from the On_Run_AnalysisProcedure and On_Finalize methods.

## Signature

```python
return_value = obj.Arguments
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    oMyArguments = oContext.Procedure.Arguments
    if oMyArguments.Exists("ChnSmoothWidth") :
        dd.ChnSmooth("[1]/[1]","/Smoothed",oMyArguments.Item("ChnSmoothWidth"),"maxNumber")
#   Enter your analysis commands
    else:
        oContext.LogError("Smooth width missing")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_Arguments_IVbsJob.htm`*
