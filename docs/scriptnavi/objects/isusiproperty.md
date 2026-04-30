---
title: "ISUSIProperty"
description: "The Property object provides in a DataFidner a property for the Root object , the ChannelGroup object , or the Channel object ."
---

# ISUSIProperty

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Property <DataFinder>

The Property object provides in a DataFidner a property for the Root object , the ChannelGroup object , or the Channel object .

## Python example

```python
dd.Navigator.Display.OpenDataFinder("My DataFinder")
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
dd.Data.Root.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchChannelgroup
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchChannelGroup,"name","=",["Dataset_005", "Dataset_010"])
oMyConditions.Logic = "C1"
oMyResultsList = oMyCurrDataProvider.ResultsList
oMyResultsElements = oMyResultsList.ResultsElements
if oMyResultsElements(1).IsKindOf(dd.eSearchChannelGroup) :
    for Channel in oMyResultsElements(1).Channels:
        dd.MsgBoxDisp(Channel.Properties("Name").Value)
```

## Members

<div markdown="1">
<div class="Properties"><div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/isusiproperty-datatype/">DataType</a> | <a href="../../properties/isusiproperty-default/">Default</a> | <a href="../../properties/isusiproperty-displayname/">DisplayName</a> | <a href="../../properties/isusiproperty-hidden/">Hidden</a> | <a href="../../properties/isusiproperty-name/">Name</a> | <a href="../../properties/isusiproperty-value/">Value</a></p>
</div>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/properties/">Properties &lt;DataFinder&gt;</a>.<a href="../../methods/isusiproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ISUSIProperty.htm`*
