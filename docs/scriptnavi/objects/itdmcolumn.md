---
title: "ITDMColumn"
description: "In the search results list of a DataFinder or of a data store the Column object provides a column with properties. If you run an advanced search, DIAdem automat"
---

# ITDMColumn

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Column

In the search results list of a DataFinder or of a data store the Column object provides a column with properties. If you run an advanced search, DIAdem automatically adds columns with the properties that you searched for. Select Configure Search Results List from the context menu of the search results list to manually add further columns with properties. You only can remove columns which were added manually.

## Python example

```python
oMyResultsList = dd.Navigator.Display.CurrDataFinder.ResultsList
oMyCell = oMyResultsList.FocusedCell
if not oMyCell is None :
    dd.MsgBoxDisp(oMyCell.Column.Property)
```

```python
oMyResultsList = dd.Navigator.Display.CurrDataStore.ResultsList
oReturnType = dd.Navigator.Display.CurrDataStore.QueryForm.ReturnType
for SelectedColumn in oMyResultsList.ColumnsSelection:
    dd.Navigator.LoadProperty(SelectedColumn.GetPath(oReturnType),oMyResultsList.Elements)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmcolumn-datatype/">DataType</a> | <a href="../../properties/itdmcolumn-property/">Property</a> | <a href="../../properties/itdmcolumn-type/">Type</a> | <a href="../../properties/itdmcolumn-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmcolumn-getpath/">GetPath</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idatafindercell/">Cell &lt;DataFinder&gt;</a>.<a href="../../properties/idatafindercell-column/">Column</a> | <a href="../idatastorecell/">Cell &lt;DataStore&gt;</a>.<a href="../../properties/idatastorecell-column/">Column</a> | <a href="../itdmcell/">Cell</a>.<a href="../../properties/itdmcell-column/">Column</a> | <a href="../../collections/columns/">Columns</a>.<a href="../../methods/itdmcolumns-add/">Add</a> | <a href="../../collections/columns/">Columns</a>.<a href="../../methods/itdmcolumns-item/">Item</a> | <a href="../../collections/columnsselection/">ColumnsSelection</a>.<a href="../../methods/itdmresultsdisplaycolumnsselection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMColumn.htm`*
