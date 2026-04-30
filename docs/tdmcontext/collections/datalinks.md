---
title: "DataLinks"
description: "Collection of all the elements of a search. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the"
---

# DataLinks

!!! abstract "Collection &middot; `TDMcontext.chm`"
    Collection: DataLinks <Analysis Automation>

Collection of all the elements of a search. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the search. Otherwise, DIAdem runs the search simultaneously, and the DataLinks <Analysis Automation> collection always contains exactly one element. If files were not indexed successfully, they are not in this collection.

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    oMyDataLinks = oContext.DataLinks
    dd.Report.LoadLayout(oContext.Procedure.ScriptPath + "MyLayout.tdr")
    for oMyDataLink in oMyDataLinks:
        dd.Navigator.LoadData(oMyDataLink)
# Enter your analysis commands
        dd.Report.Sheets.ExportToPDF(oContext.Procedure.Arguments.Item("ResultsPath").Value + dd.Data.Root.Properties("name").Value + ".pdf")
# Enter your analysis commands
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbsdatalinkscollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbsdatalinkscollection-getasarray/">GetAsArray</a> | <a href="../../methods/ivbsdatalinkscollection-getenumerator/">GetEnumerator</a> | <a href="../../methods/ivbsdatalinkscollection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-datalinks/">DataLinks</a> | <a href="../../objects/ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-datalinks/">DataLinks</a> | <a href="../../objects/ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-datalinks/">DataLinks</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsDataLinksCollection.htm`*
