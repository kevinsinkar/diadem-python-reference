---
title: "IVbsStatus.On_Run_AnalysisProcedure_Success"
description: "Receives the information whether the On_Run_AnalysisProcedure procedure for analyzing the data was successful."
---

# IVbsStatus.On_Run_AnalysisProcedure_Success

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: On_Run_AnalysisProcedure_Success for Status <Analysis Automation>

Receives the information whether the On_Run_AnalysisProcedure procedure for analyzing the data was successful.

## Signature

```python
obj.On_Run_AnalysisProcedure_Success
```

## Python example

```python
def On_Finalize(oContext):
    if not oContext.Status.On_Initialize_Success :
        oContext.LogError("Init not ok")
    if not oContext.Status.On_Run_AnalysisProcedure_Success :
        oContext.LogError("Analysis not ok")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_On_Run_AnalysisProcedure_Success_IVbsStatus.htm`*
