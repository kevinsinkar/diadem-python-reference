---
title: "IDisplay.OpenDataStore"
description: "Opens a data store in the DIAdem NAVIGATOR interface."
---

# IDisplay.OpenDataStore

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: OpenDataStore for Display

Opens a data store in the DIAdem NAVIGATOR interface.

## Signature

```python
bOpenDataStore = Object.OpenDataStore(Name)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If DIAdem cannot execute the <span class="Monospace">OpenDataStore</span> method successfully, DIAdem fills the VBS Error object and aborts the script. DIAdem writes further information into the logfile and displays a dialog box that contains information on the error.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use <span class="Monospace">Navigator.Display.CurrDataStore</span> to access the DataStore object.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <span class="Monospace">GetDataStore</span> method to determine the associated data store without interface for a data store, which already has an open interface. Use the <span class="Monospace">ConnectDataStore</span> method to work directly with a data store without a user interface.</td></tr></table>
</div>

## Python example

```python
dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
```

```python
if dd.Navigator.Display.CurrDataStore is None :
    dd.Navigator.Display.OpenDataStore("ASAM Browse Settings Example")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_OpenDataStore_IDisplay.htm`*
