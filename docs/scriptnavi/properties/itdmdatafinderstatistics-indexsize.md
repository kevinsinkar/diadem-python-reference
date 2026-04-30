---
title: "ITDMDataFinderStatistics.IndexSize"
description: "Displays the size in kilobyte (kB) of the index which the DataFinder generated when indexing the search area."
---

# ITDMDataFinderStatistics.IndexSize

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IndexSize for DataFinderStatistics

Displays the size in kilobyte (kB) of the index which the DataFinder generated when indexing the search area.

## Signature

```python
obj.IndexSize
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyIndexer = oMyDataFinder.Indexer
oMyStatistics = oMyIndexer.GetStatistics()
dd.MsgBoxDisp ("Last Index Completion: " + oMyStatistics.LastCompleteIndexing.VariantDate  + "\r\n" + "Indexing Complete: " + oMyStatistics.IndexingComplete  + "\r\n" + "Analyzed Files: " + oMyStatistics.AnalyzedFiles + "\r\n" + "Indexed Files: " + oMyStatistics.IndexedFiles  + "\r\n" + "Indexed Groups: " + oMyStatistics.IndexedGroups  + "\r\n" + "Indexed Channels: " + oMyStatistics.IndexedChannels + "\r\n" + "Index Size [kB]: " + oMyStatistics.IndexSize)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IndexSize_ITDMDataFinderStatistics.htm`*
