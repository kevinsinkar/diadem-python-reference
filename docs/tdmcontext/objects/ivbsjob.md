---
title: "IVbsJob"
description: "The Procedure <Analysis Automation> object provides information on the current procedure being executed."
---

# IVbsJob

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: Procedure <Analysis Automation>

The Procedure <Analysis Automation> object provides information on the current procedure being executed.

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
<p><a href="../../properties/ivbsjob-arguments/">Arguments</a> | <a href="../../properties/ivbsjob-scriptpath/">ScriptPath</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-procedure/">Procedure</a> | <a href="../ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-procedure/">Procedure</a> | <a href="../ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-procedure/">Procedure</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsJob.htm`*
