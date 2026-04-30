---
title: "Conditions"
description: "Collection of the search parameters for an advanced search in a DataFinder."
---

# Conditions

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: Conditions <DataFinder>

Collection of the search parameters for an advanced search in a DataFinder.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to the help page <a href="#" data-unresolved="1">Properties - Overview</a> for an overview of the the interface terms, the script name, and the meanings of the properties of files, groups, and channels. You need the language-neutral script name of a property when you use a script to search for the value of a property. You also can enter a query in the search input area in DIAdem NAVIGATOR and press &lt;Ctrl-Shift-C&gt; to find the script name of a property. Then DIAdem saves a script to the clipboard that also contains the script name of the property.</td></tr></table>
</div>

## Python example

```python
oMyQueryForm = dd.Navigator.Display.CurrDataFinder.QueryForm
if oMyQueryForm.Mode == dd.eAdvancedQuery :
    Conditions = oMyQueryForm.Conditions
    for Condition in Conditions:
        if sLogic == "" :
            sLogic = Condition.Name
        else:
            sLogic = sLogic + " or " + Condition.Name
    Conditions.Logic = sLogic
```

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
if oMyQuery.IsKindOf(dd.eAdvancedQuery) :
    Conditions = oMyQuery.Conditions
    Index = 1
    for Condition in Conditions:
        if Condition.Type == dd.eSearchChannel :
            Conditions.Remove(Index)
        else:
            dd.MsgBoxDisp (Condition.Property + Condition.Operator + Condition.Value)
            Index = Index +1
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmdatafinderconditions-count/">Count</a> | <a href="../../properties/itdmdatafinderconditions-logic/">Logic</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmdatafinderconditions-add/">Add</a> | <a href="../../methods/itdmdatafinderconditions-item/">Item</a> | <a href="../../methods/itdmdatafinderconditions-remove/">Remove</a> | <a href="../../methods/itdmdatafinderconditions-removeall/">RemoveAll</a> | <a href="../../methods/itdmdatafinderconditions-renumber/">Renumber</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmdatafinderadvancedquery/">AdvancedQuery &lt;DataFinder&gt;</a>.<a href="../../properties/itdmdatafinderadvancedquery-conditions/">Conditions</a> | <a href="../../objects/inavidatafinderqueryform/">QueryForm &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderqueryform-conditions/">Conditions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMDataFinderConditions.htm`*
