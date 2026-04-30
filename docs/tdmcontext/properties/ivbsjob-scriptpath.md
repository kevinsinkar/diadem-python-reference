---
title: "IVbsJob.ScriptPath"
description: "Returns the current temporary script path of the procedure currently being executed. This path also contains the other files from the analysis automation proced"
---

# IVbsJob.ScriptPath

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: ScriptPath for Procedure <Analysis Automation>

Returns the current temporary script path of the procedure currently being executed. This path also contains the other files from the analysis automation procedure.

## Signature

```python
obj.ScriptPath
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_ScriptPath_IVbsJob.htm`*
