---
title: "IVbsContextASDeinit.LogWarning"
description: "Creates a warning. The analysis automation continues the script."
---

# IVbsContextASDeinit.LogWarning

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: LogWarning for ContextFinalize <Analysis Automation>

Creates a warning. The analysis automation continues the script.

## Signature

```python
obj.LogWarning(message)
```

## Python example

```python
def On_Finalize(oContext):
    oMyArguments = oContext.Procedure.Arguments
    if oMyArguments.Exists("ResultsPath") :
        ResultsPath = oMyArguments.Item("ResultsPath").Value
        oContext.LogResult("Results path: " + ResultsPath)
    else:
        oContext.LogWarning("Results path missing")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_LogWarning_IVbsContextASDeinit.htm`*
