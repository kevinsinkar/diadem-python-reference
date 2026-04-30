---
title: "ITDMDataFinderAdvancedQuery"
description: "The AdvancedQuery object provides the properties of an Advanced search in a DataFinder. If you run an advanced search, DIAdem searches for the property values o"
---

# ITDMDataFinderAdvancedQuery

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: AdvancedQuery <DataFinder>

The AdvancedQuery object provides the properties of an Advanced search in a DataFinder. If you run an advanced search, DIAdem searches for the property values of the files, groups, or channels that you selected.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If you enter parameters for an advanced search in the DIAdem NAVIGATOR interface and press &lt;Ctrl-Shift-C&gt;, DIAdem saves a script for the use of the <span class="Monospace">AdvancedQuery</span> object to the clipboard.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyAdvancedQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyAdvancedQuery.ReturnType = dd.eSearchChannel
oMyAdvancedQuery.Conditions.Add(dd.eSearchChannelGroup, "name", "=", "Dataset_001")
oMyDataFinder.Search(oMyAdvancedQuery)
oMyResults = oMyDataFinder.ResultsElements
dd.Navigator.LoadData(oMyResults)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafinderadvancedquery-conditions/">Conditions</a> | <a href="../../properties/itdmdatafinderadvancedquery-returntype/">ReturnType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatafinderadvancedquery-isempty/">IsEmpty</a> | <a href="../../methods/itdmdatafinderadvancedquery-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatafinder/">DataFinder</a>.<a href="../../methods/itdmdatafinder-createquery/">CreateQuery</a> | <a href="../itdmdatafinder/">DataFinder</a>.<a href="../../methods/itdmdatafinder-loadquery/">LoadQuery</a> | <a href="../inavidatafinderqueryform/">QueryForm &lt;DataFinder&gt;</a>.<a href="../../methods/inavidatafinderqueryform-getcurrquery/">GetCurrQuery</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../idatafinderquery/">Query</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinderAdvancedQuery.htm`*
