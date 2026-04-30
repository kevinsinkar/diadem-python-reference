---
title: "IVbsContextASInit.RaiseError"
description: "Terminates the On_Initialize event with an error message without executing further commands. In a parallel analysis, Analysis Automation executes the On_Finaliz"
---

# IVbsContextASInit.RaiseError

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: RaiseError for ContextInitialize <Analysis Automation>

Terminates the On_Initialize event with an error message without executing further commands. In a parallel analysis, Analysis Automation executes the On_Finalize event afterwards anyway.

## Signature

```python
obj.RaiseError(errNumber, message)
```

## Python example

```python
def On_Initialize(oContext):
    oMyArguments = oContext.Procedure.Arguments
    if oMyArguments.Exists("ResultsPath") :
        ResultsPath = oMyArguments.Item("ResultsPath").Value
        oContext.LogResult("Results path: " + ResultsPath)
    else:
        oContext.RaiseError(1,"Results path missing")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_RaiseError_IVbsContextASInit.htm`*
