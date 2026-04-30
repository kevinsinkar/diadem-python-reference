---
title: "Arguments"
description: "The Arguments <SystemLink> object provides the list of arguments in Data Preparation or Analysis Automation."
---

# Arguments

!!! abstract "Collection &middot; `TDMcontext.chm`"
    Collection: Arguments <SystemLink>

The Arguments <SystemLink> object provides the list of arguments in Data Preparation or Analysis Automation.

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    oMyDataLinks = oContext.DataLinks
    dd.Report.LoadLayout(oContext.Procedure.ScriptPath + "MyLayout.tdr")
    for oMyDataLink in oMyDataLinks:
        dd.Navigator.LoadData(oMyDataLink)
# Enter your analysis commands
        dd.Report.Sheets.ExportToPDF(oContext.Procedure.Arguments.Item("ResultsPath").Value + dd.Data.Root.Properties("name").Value + ".pdf", True)
# Enter your analysis commands
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbsargumentcollection-item/">Item</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbsargumentcollection-add/">Add</a> | <a href="../../methods/ivbsargumentcollection-count/">Count</a> | <a href="../../methods/ivbsargumentcollection-exists/">Exists</a> | <a href="../../methods/ivbsargumentcollection-getenumerator/">GetEnumerator</a> | <a href="../../methods/ivbsargumentcollection-getorcreate/">GetOrCreate</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-dynamicarguments/">DynamicArguments</a> | <a href="../../objects/ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-dynamicarguments/">DynamicArguments</a> | <a href="../../objects/ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-dynamicarguments/">DynamicArguments</a> | <a href="../../objects/ivbscontextvnv/">ContextVnV &lt;Data Preprocessor&gt;</a>.<a href="../../properties/ivbscontextvnv-arguments/">Arguments</a> | <a href="../../objects/ivbsjob/">Procedure &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbsjob-arguments/">Arguments</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsArgumentCollection.htm`*
