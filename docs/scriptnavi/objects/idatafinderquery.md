---
title: "IDataFinderQuery"
description: "The Query provides a search object in a DataFinder. You can use this search object for a Search with the interface of DIAdem NAVIGATOR and for a Search without "
---

# IDataFinderQuery

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Query <DataFinder>

The Query provides a search object in a DataFinder. You can use this search object for a Search with the interface of DIAdem NAVIGATOR and for a Search without the interface . You can run a Quick search and an Advanced search with this search object.

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQuery = oMyCurrDataProvider.QueryForm.GetCurrQuery()
if (oMyQuery.IsKindOf(dd.eTextQuery)) :
    dd.MsgBoxDisp(oMyQuery.Text)
else:
    dd.MsgBoxDisp("Advanced Query")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatafinderquery-returntype/">ReturnType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatafinderquery-isempty/">IsEmpty</a> | <a href="../../methods/idatafinderquery-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatafinder/">DataFinder</a>.<a href="../../methods/itdmdatafinder-createquery/">CreateQuery</a> | <a href="../itdmdatafinder/">DataFinder</a>.<a href="../../methods/itdmdatafinder-loadquery/">LoadQuery</a> | <a href="../inavidatafinderqueryform/">QueryForm &lt;DataFinder&gt;</a>.<a href="../../methods/inavidatafinderqueryform-getcurrquery/">GetCurrQuery</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="../itdmdatafinderadvancedquery/">AdvancedQuery</a> | <a href="../itdmdatafindertextquery/">TextQuery</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataFinderQuery.htm`*
