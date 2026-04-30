---
title: "IVbsArgument"
description: "The Argument <SystemLink> object provides an argument in Data Preparation or Analysis Automation."
---

# IVbsArgument

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: Argument <SystemLink>

The Argument <SystemLink> object provides an argument in Data Preparation or Analysis Automation.

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
<p><a href="../../properties/ivbsargument-description/">Description</a> | <a href="../../properties/ivbsargument-name/">Name</a> | <a href="../../properties/ivbsargument-type/">Type</a> | <a href="../../properties/ivbsargument-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/arguments/">Arguments &lt;SystemLink&gt;</a>.<a href="../../methods/ivbsargumentcollection-add/">Add</a> | <a href="../../collections/arguments/">Arguments &lt;SystemLink&gt;</a>.<a href="../../methods/ivbsargumentcollection-getorcreate/">GetOrCreate</a> | <a href="../../collections/arguments/">Arguments &lt;SystemLink&gt;</a>.<a href="../../properties/ivbsargumentcollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsArgument.htm`*
