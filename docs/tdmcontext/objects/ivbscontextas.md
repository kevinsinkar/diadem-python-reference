---
title: "IVbsContextAS"
description: "The ContextRun <Analysis Automation> object provides information on the analysis automation event On_Run_AnalysisProcedure . The On_Run_AnalysisProcedure event "
---

# IVbsContextAS

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: ContextRun <Analysis Automation>

The ContextRun <Analysis Automation> object provides information on the analysis automation event On_Run_AnalysisProcedure . The On_Run_AnalysisProcedure event is called several times if you execute a parallel analysis, otherwise it is called only once.

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    oMyDataLinks = oContext.DataLinks
    for iCount in range( 1, oMyDataLinks.Count+1):
        dd.Navigator.LoadData(oContext.DataLinks.Item(iCount))
# Enter your analysis commands
# Enter your analysis commands
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbscontextas-currdataprovider/">CurrDataProvider</a> | <a href="../../properties/ivbscontextas-datalinks/">DataLinks</a> | <a href="../../properties/ivbscontextas-dynamicarguments/">DynamicArguments</a> | <a href="../../properties/ivbscontextas-fileservice/">FileService</a> | <a href="../../properties/ivbscontextas-procedure/">Procedure</a> | <a href="../../properties/ivbscontextas-tags/">Tags</a> | <a href="../../properties/ivbscontextas-taskexecution/">TaskExecution</a> | <a href="../../properties/ivbscontextas-tempfolder/">TempFolder</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbscontextas-logerror/">LogError</a> | <a href="../../methods/ivbscontextas-logresult/">LogResult</a> | <a href="../../methods/ivbscontextas-logwarning/">LogWarning</a> | <a href="../../methods/ivbscontextas-raiseerror/">RaiseError</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsContextAS.htm`*
