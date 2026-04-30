---
title: "IVbsContextAS.LogError"
description: "Creates an error. The analysis automation continues the script but marks the file in the analysis automation as failed."
---

# IVbsContextAS.LogError

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: LogError for ContextRun  <Analysis Automation>

Creates an error. The analysis automation continues the script but marks the file in the analysis automation as failed.

## Signature

```python
obj.LogError(message)
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    oMyArguments = oContext.Procedure.Arguments
    if oMyArguments.Exists("ResultsPath") :
        ResultsPath = oMyArguments.Item("ResultsPath").Value
        oContext.LogResult("Results path: " + ResultsPath)
    else:
        oContext.LogError("Resultpath missing")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_LogError_IVbsContextAS.htm`*
