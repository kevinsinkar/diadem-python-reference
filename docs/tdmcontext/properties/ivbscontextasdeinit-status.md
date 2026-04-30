---
title: "IVbsContextASDeinit.Status"
description: "Returns the Status <Analysis Automation> object which contains the information whether the methods On_ Initialize and On_Run_AnalysisProcedure were successful."
---

# IVbsContextASDeinit.Status

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Status for ContextFinalize <Analysis Automation>

Returns the Status <Analysis Automation> object which contains the information whether the methods On_ Initialize and On_Run_AnalysisProcedure were successful.

## Signature

```python
return_value = obj.Status
```

## Python example

```python
def On_Finalize(oContext):
    oContext.LogResult("Init ok: " + oContext.Status.On_Initialize_Success)
    oContext.LogResult("Analysis ok: " + oContext.Status.On_Run_AnalysisProcedure_Success)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_Status_IVbsContextASDeinit.htm`*
