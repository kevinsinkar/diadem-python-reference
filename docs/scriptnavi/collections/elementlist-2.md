---
title: "ElementList"
description: "Unsorted collection of data elements from a data store. For example, the collection can contain search results or selected elements."
---

# ElementList

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ElementList <DataStore>

Unsorted collection of data elements from a data store. For example, the collection can contain search results or selected elements.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <span class="Monospace">GetElementList</span> method to create a list of elements that meet the condition specified as a parameter.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyElementList = oMyDataStore.GetElementList("MeaQuantity", "maximum<13")
for Element in oMyElementList:
    dd.MsgBoxDisp(Element.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmstoreelementlist-count/">Count</a> | <a href="../../properties/itdmstoreelementlist-isincomplete/">IsIncomplete</a> | <a href="../../properties/itdmstoreelementlist-maxcount/">MaxCount</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmstoreelementlist-item/">Item</a> | <a href="../../methods/itdmstoreelementlist-sort/">Sort</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavidatastorebrowser/">Browser &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastorebrowser-selectedelements/">SelectedElements</a> | <a href="../../objects/itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-getelementlist/">GetElementList</a> | <a href="../../objects/itdmdatastore/">DataStore</a>.<a href="../../properties/itdmdatastore-resultselements/">ResultsElements</a> | <a href="../../objects/inavidatastoreresultdisplay/">ResultsList &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastoreresultdisplay-resultselements/">ResultsElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMStoreElementList.htm`*
