---
title: "IVbsContextASDeinit"
description: "The ContextFinalize <Analysis Automation> object provides information on the analysis automation event On_Finalize . The On_Finalize event is only called if you"
---

# IVbsContextASDeinit

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: ContextFinalize <Analysis Automation>

The ContextFinalize <Analysis Automation> object provides information on the analysis automation event On_Finalize . The On_Finalize event is only called if you execute a parallel analysis.

## Python example

```python
def On_Finalize(oContext):
    oContext.LogResult("Init ok: " + oContext.Status.On_Initialize_Success)
    oContext.LogResult("Analysis ok: " + oContext.Status.On_Run_AnalysisProcedure_Success)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbscontextasdeinit-currdataprovider/">CurrDataProvider</a> | <a href="../../properties/ivbscontextasdeinit-datalinks/">DataLinks</a> | <a href="../../properties/ivbscontextasdeinit-dynamicarguments/">DynamicArguments</a> | <a href="../../properties/ivbscontextasdeinit-fileservice/">FileService</a> | <a href="../../properties/ivbscontextasdeinit-procedure/">Procedure</a> | <a href="../../properties/ivbscontextasdeinit-status/">Status</a> | <a href="../../properties/ivbscontextasdeinit-tags/">Tags</a> | <a href="../../properties/ivbscontextasdeinit-taskexecution/">TaskExecution</a> | <a href="../../properties/ivbscontextasdeinit-tempfolder/">TempFolder</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbscontextasdeinit-logerror/">LogError</a> | <a href="../../methods/ivbscontextasdeinit-logresult/">LogResult</a> | <a href="../../methods/ivbscontextasdeinit-logwarning/">LogWarning</a> | <a href="../../methods/ivbscontextasdeinit-raiseerror/">RaiseError</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsContextASDeinit.htm`*
