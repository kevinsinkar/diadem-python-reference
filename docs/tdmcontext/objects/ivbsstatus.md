---
title: "IVbsStatus"
description: "The Status <Analysis Automation> object provides the information on whether the events On_Initialize and On_Run_AnalysisProcedure were successful. The event On_"
---

# IVbsStatus

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: Status <Analysis Automation>

The Status <Analysis Automation> object provides the information on whether the events On_Initialize and On_Run_AnalysisProcedure were successful. The event On_Finalize is always called, even if the events On_Initialize and On_Run_AnalysisProcedure were not successful.

## Python example

```python
def On_Finalize(oContext):
    oContext.LogResult("Init ok: " + oContext.Status.On_Initialize_Success)
    oContext.LogResult("Analysis ok: " + oContext.Status.On_Run_AnalysisProcedure_Success)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbsstatus-on-initialize-success/">On_Initialize_Success</a> | <a href="../../properties/ivbsstatus-on-run-analysisprocedure-success/">On_Run_AnalysisProcedure_Success</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-status/">Status</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsStatus.htm`*
