---
title: "ITDMDataFinderTextQuery"
description: "The TextQuery object provides the properties for a quick search in a DataFinder. If you run a quick search, DIAdem searches all the properties of the files, gro"
---

# ITDMDataFinderTextQuery

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: TextQuery <DataFinder>

The TextQuery object provides the properties for a quick search in a DataFinder. If you run a quick search, DIAdem searches all the properties of the files, groups, and channels from the search areas for the specified value.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If you enter a search term for the quick search in the DIAdem NAVIGATOR interface and press &lt;Ctrl-Shift-C&gt;, DIAdem saves a script for using the <span class="Monospace">TextQuery</span> object to the clipboard.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()
oMyCurrDataProvider = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyCurrDataProvider.CreateQuery(dd.eTextQuery)
oMyQuery.Text = "Brake*"
oMyCurrDataProvider.SearchElements(oMyQuery)
oMyResults = oMyCurrDataProvider.ResultsElements
for Element in oMyResults:
    Output = Output + "\r\n" + Element.Name
dd.MsgBoxDisp("Results Elements: " + Output)
dd.Navigator.LoadData(oMyResults)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafindertextquery-returntype/">ReturnType</a> | <a href="../../properties/itdmdatafindertextquery-text/">Text</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatafindertextquery-isempty/">IsEmpty</a> | <a href="../../methods/itdmdatafindertextquery-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavidatafinderqueryform/">QueryForm</a>.<a href="../../methods/inavidatafinderqueryform-getcurrquery/">GetCurrQuery</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../idatafinderquery/">Query &lt;DataFinder&gt;</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinderTextQuery.htm`*
