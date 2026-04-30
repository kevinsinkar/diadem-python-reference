---
title: "ITDMDataFinderIndexer"
description: "The Indexer object provides the methods which you use to reindex files and folders of the My DataFinder DataFinder. You cannot use the indexer object for DataFi"
---

# ITDMDataFinderIndexer

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Indexer

The Indexer object provides the methods which you use to reindex files and folders of the My DataFinder DataFinder. You cannot use the indexer object for DataFinders that are located on another host.

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyIndexer = oMyDataFinder.Indexer
oMyStatistics = oMyIndexer.GetStatistics()
dd.MsgBoxDisp ("Last Index Completion: " + oMyStatistics.LastCompleteIndexing.VariantDate  + "\r\n" + "Indexing Complete: " + oMyStatistics.IndexingComplete  + "\r\n" + "Analyzed Files: " + oMyStatistics.AnalyzedFiles + "\r\n" + "Indexed Files: " + oMyStatistics.IndexedFiles  + "\r\n" + "Indexed Groups: " + oMyStatistics.IndexedGroups  + "\r\n" + "Indexed Channels: " + oMyStatistics.IndexedChannels + "\r\n" + "Index Size: " + oMyStatistics.IndexSize)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafinderindexer-status/">Status</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatafinderindexer-getstatistics/">GetStatistics</a> | <a href="../../methods/itdmdatafinderindexer-indexfile/">IndexFile</a> | <a href="../../methods/itdmdatafinderindexer-indexfolder/">IndexFolder</a> | <a href="../../methods/itdmdatafinderindexer-reindexelement/">ReindexElement</a> | <a href="../../methods/itdmdatafinderindexer-reindexplugin/">ReindexPlugin</a> | <a href="../../methods/itdmdatafinderindexer-updateindex/">UpdateIndex</a> | <a href="../../methods/itdmdatafinderindexer-updatesearcharea/">UpdateSearchArea</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatafinder/">DataFinder</a>.<a href="../../properties/itdmdatafinder-indexer/">Indexer</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinderIndexer.htm`*
