---
title: "ITDMDataFinderIndexer.IndexFile"
description: "Indexes the specified file in a DataFinder. You can use this method only on the computer on which the DataFinder is active."
---

# ITDMDataFinderIndexer.IndexFile

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IndexFile for Indexer

Indexes the specified file in a DataFinder. You can use this method only on the computer on which the DataFinder is active.

## Signature

```python
eIndexFile = Object.IndexFile(Path, Reindex, WaitTime)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you call the <span class="Monospace">IndexFile</span> method while the DataFinder is executing an indexing process specified by a scheduler, the DataFinder interrupts the indexing of the scheduler and first executes the method. Then the DataFinder continues the indexing process specified by the scheduler.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you stop the indexing process of the DataFinder, the <span class="Monospace">IndexFile</span> method is interrupted until you continue the indexing of the DataFinder.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can use the <span class="Monospace">IndexFile</span> method from Version 2.2 of the DataFinder.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eIndexedNotYet` | 0 | The file has not been indexed yet. |
| `eIndexedFailure` | 1 | An error has occurred during indexing. Refer to the properties display in the search results list through the Error message property. |
| `eIndexedSuccess` | 2 | The file has been indexed. |
| `eIndexedTimeout` | 3 | The time allowed for indexing in seconds has been exceeded. |
| `eIndexedNotMyFile` | 4 | The file has a file extension for which a DataPlugin is registered. However the file format does not match this DataPlugin. |
| `eIndexedUnknown` | 100 | The index status is unknown. |

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyIndexer = oMyDataFinder.Indexer
oMyIndexer.IndexFile("C:\\MySearchArea\\MyData\\MyFile.tdm",True,5)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/Navigator_method_IndexFile_ITDMDataFinderIndexer.htm`*
