---
title: "IVbsContextASDeinit.RaiseError"
description: "Terminates the On_Finalize event with an error message without executing further commands."
---

# IVbsContextASDeinit.RaiseError

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: RaiseError for ContextFinalize <Analysis Automation>

Terminates the On_Finalize event with an error message without executing further commands.

## Signature

```python
obj.RaiseError(errNumber, message)
```

## Python example

```python
def On_Finalize(oContext):
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

*Source: `TDMcontext/methods/TDMContext_method_RaiseError_IVbsContextASDeinit.htm`*
