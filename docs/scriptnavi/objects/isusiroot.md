---
title: "ISUSIRoot"
description: "The Root object provides a file in a DataFinder. Thus the Element object is a file."
---

# ISUSIRoot

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Root <DataFinder>

The Root object provides a file in a DataFinder. Thus the Element object is a file.

## Python example

```python
dd.Navigator.Display.OpenDataFinder("My DataFinder")
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
dd.Data.Root.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyResultsList = oMyCurrDataProvider.ResultsList
oMyResultsElements = oMyResultsList.ResultsElements
for Element in oMyResultsElements:
    if Element.IsKindOf(dd.eSearchFile) :
        Output = Output + "\r\n" + Element.Name
dd.MsgBoxDisp("File names: " + Output)
dd.Navigator.LoadData(oMyResultsElements)
```

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
for Element in oMyResultsElements:
    if Element.IsKindOf(dd.eSearchChannelgroup) :
        dd.MsgBoxDisp(Element.Root.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/isusiroot-channelgroups/">ChannelGroups</a> | <a href="../../properties/isusiroot-name/">Name</a> | <a href="../../properties/isusiroot-properties/">Properties</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/isusiroot-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavidatafinderbrowser/">Browser &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderbrowser-focusedelement/">FocusedElement</a> | <a href="../idatafindercell/">Cell &lt;DataFinder&gt;</a>.<a href="../../properties/idatafindercell-element/">Element</a> | <a href="../isusichannelgroup/">ChannelGroup &lt;DataFinder&gt;</a>.<a href="../../properties/isusichannelgroup-root/">Root</a> | <a href="../../collections/elementlist/">ElementList &lt;DataFinder&gt;</a>.<a href="../../methods/isusielements-item/">Item</a> | <a href="../../collections/elementsselection/">ElementsSelection &lt;DataFinder&gt;</a>.<a href="../../methods/idatafinderresultsdisplayelementsselection-item/">Item</a> | <a href="../../collections/freeelementlist/">FreeElementList &lt;DataFinder&gt;</a>.<a href="../../methods/itdmfreedatafinderelementlist-add/">Add</a> | <a href="../../collections/freeelementlist/">FreeElementList &lt;DataFinder&gt;</a>.<a href="../../methods/itdmfreedatafinderelementlist-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Obects Overview</a> | <a href="#" data-unresolved="1">Properties in DIAdem - Overview</a> | <a href="../isusielement/">Element</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ISUSIRoot.htm`*
