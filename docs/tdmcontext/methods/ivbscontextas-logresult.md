---
title: "IVbsContextAS.LogResult"
description: "Creates a result text. The analysis automation continues the script."
---

# IVbsContextAS.LogResult

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: LogResult for ContextRun <Analysis Automation>

Creates a result text. The analysis automation continues the script.

## Signature

```python
obj.LogResult(message)
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
# Enter your analysis commands
    oContext.LogResult("Results path: " + ResultsPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_LogResult_IVbsContextAS.htm`*
