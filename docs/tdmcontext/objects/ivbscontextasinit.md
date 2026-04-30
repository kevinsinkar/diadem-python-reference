---
title: "IVbsContextASInit"
description: "The ContextInitialize <Analysis Automation> object provides information on the analysis automation event On_Initialize . The On_Initialize event is only called "
---

# IVbsContextASInit

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: ContextInitialize <Analysis Automation>

The ContextInitialize <Analysis Automation> object provides information on the analysis automation event On_Initialize . The On_Initialize event is only called if you execute a parallel analysis.

## Python example

```python
def On_Initialize(oContext):
    if oContext.Procedure.Arguments.Exists("ResultsPath") :
        ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
        oContext.LogResult("Results path: " + ResultsPath)
    else:
        oContext.LogError("Results path missing")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbscontextasinit-currdataprovider/">CurrDataProvider</a> | <a href="../../properties/ivbscontextasinit-datalinks/">DataLinks</a> | <a href="../../properties/ivbscontextasinit-dynamicarguments/">DynamicArguments</a> | <a href="../../properties/ivbscontextasinit-fileservice/">FileService</a> | <a href="../../properties/ivbscontextasinit-procedure/">Procedure</a> | <a href="../../properties/ivbscontextasinit-tags/">Tags</a> | <a href="../../properties/ivbscontextasinit-taskexecution/">TaskExecution</a> | <a href="../../properties/ivbscontextasinit-tempfolder/">TempFolder</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbscontextasinit-logerror/">LogError</a> | <a href="../../methods/ivbscontextasinit-logwarning/">LogWarning</a> | <a href="../../methods/ivbscontextasinit-raiseerror/">RaiseError</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsContextASInit.htm`*
