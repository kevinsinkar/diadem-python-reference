---
title: "IDataStoreDisplay.LoadQueryInfoSet"
description: "Loads in a data store a file with the filename extension .tdq . DIAdem saves queries and the configuration of the search results list in TDQ files. Note Use the"
---

# IDataStoreDisplay.LoadQueryInfoSet

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadQueryInfoSet for DataStoreDisplay

Loads in a data store a file with the filename extension .tdq . DIAdem saves queries and the configuration of the search results list in TDQ files. Note Use the LoadQuery method instead of the LoadQueryInfoSet method if you want to work on the DIAdem NAVIGATOR interface.

## Signature

```python
eLoadQueryInfoSet = Object.LoadQueryInfoSet(FilePathName, [QueryInfoSetMode])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="../itdmdatastore-loadquery/">LoadQuery</a> method instead of the <span class="Monospace">LoadQueryInfoSet</span> method if you want to work on the DIAdem NAVIGATOR interface.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eQISModeQuery` | 24001 | Loads only the query from the TDQ file. |
| `eQISModeResultsList` | 24002 | Loads only the settings of the search results list from the TDQfile. |
| `eQISModeInfoSet` | 24008 | Loads all information from the TDQ file. |

## Python example

```python
cQueryInfoSetModeIn = dd.eQISModeQuery

cQueryInfoSetMode = dd.Navigator.Display.CurrDataStore.LoadQueryInfoSet(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq", cQueryInfoSetModeIn)
dd.MsgBoxDisp("Loaded part of query info : " + QueryInfoSetModeToText (cQueryInfoSetMode) + "\r\n" + "Requested: " + QueryInfoSetModeToText (cQueryInfoSetModeIn))

def QueryInfoSetModeToText(cQueryInfoSetMode):
    select_variable_0 = cQueryInfoSetMode
    if (select_variable_0 == dd.eQISModeInfoSet) :
        sTxt = "QueryInfoSet"
    elif (select_variable_0 == dd.eQISModeQuery) :
        sTxt = "Query"
    elif (select_variable_0 == dd.eQISModeResultsList) :
        sTxt = "ResultsList"
    QueryInfoSetModeToText = sTxt
    return QueryInfoSetModeToText
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadQueryInfoSet_IDataStoreDisplay.HTM`*
