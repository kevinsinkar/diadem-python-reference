---
title: "IVbsDataLinksCollection.Item"
description: "Returns an individual element of the DataLinks <Analysis Automation> collection. You load the element with LoadData for Navigator . Accessing data through the n"
---

# IVbsDataLinksCollection.Item

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: Item for DataLinks <Analysis Automation>

Returns an individual element of the DataLinks <Analysis Automation> collection. You load the element with LoadData for Navigator . Accessing data through the network may be slow. To load all retrieved elements at the same time, you can use the GetAsArray for DataLinks method. The GetAsArray method may use a lot of memory because analysis automation loads all retrieved data simultaneously.

## Signature

```python
sItem = Object.Item(index)
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

*Source: `TDMcontext/methods/TDMContext_method_Item_IVbsDataLinksCollection.htm`*
