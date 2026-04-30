---
title: "ITDMStoreElement"
description: "The Element object provides a data element in a data store. A data element is a specific instance of an entity."
---

# ITDMStoreElement

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Element <DataStore>

The Element object provides a data element in a data store. A data element is a specific instance of an entity.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="../itdmstoreelementwithbulk/">ElementWithValues</a> object with the associated methods and properties if the data element was derived from the <span class="Monospace">AOLocalColumn</span> type.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Working with the Elements Collection and the Element Object</a> for general information on working with the elements.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyRootElement = oMyDataStore.RootElements(1)
oMyElements = oMyRootElement.Children
for Element in oMyElements:
    Output = Output + "\r\n" + Element.Name
dd.MsgBoxDisp("Name of children elements: " + Output)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmstoreelement-children/">Children</a> | <a href="../../properties/itdmstoreelement-displayname/">DisplayName</a> | <a href="../../properties/itdmstoreelement-instancekey/">InstanceKey</a> | <a href="../../properties/itdmstoreelement-name/">Name</a> | <a href="../../properties/itdmstoreelement-parent/">Parent</a> | <a href="../../properties/itdmstoreelement-properties/">Properties</a> | <a href="../../properties/itdmstoreelement-references/">References</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmstoreelement-getdatafinderinfo/">GetDataFinderInfo</a> | <a href="../../methods/itdmstoreelement-iskindof/">IsKindOf</a> | <a href="../../methods/itdmstoreelement-isvalid/">IsValid</a> | <a href="../../methods/itdmstoreelement-refresh/">Refresh</a> | <a href="../../methods/itdmstoreelement-save/">Save</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavidatastorebrowser/">Browser &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastorebrowser-focusedelement/">FocusedElement</a> | <a href="../itdmbrowsesettings/">BrowseSettings</a>.<a href="../../methods/itdmbrowsesettings-getparent/">GetParent</a> | <a href="../idatastorecell/">Cell &lt;DataStore&gt;</a>.<a href="../../properties/idatastorecell-element/">Element</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-createelement/">CreateElement</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-getelementbydatachannel/">GetElementByDataChannel</a> | <a href="../itdmdatastore/">DataStore</a>.<a href="../../methods/itdmdatastore-getelementbykey/">GetElementByKey</a> | <a href="./">Element &lt;DataStore&gt;</a>.<a href="../../properties/itdmstoreelement-parent/">Parent</a> | <a href="../../collections/elementlist-2/">ElementList &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelementlist-item/">Item</a> | <a href="../../collections/elements/">Elements &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelements-add/">Add</a> | <a href="../../collections/elements/">Elements &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelements-addreference/">AddReference</a> | <a href="../../collections/elements/">Elements &lt;DataStore&gt;</a>.<a href="../../methods/itdmstoreelements-item/">Item</a> | <a href="../../collections/elementsselection-2/">ElementsSelection &lt;DataStore&gt;</a>.<a href="../../methods/idatastoreresultsdisplayelementsselection-item/">Item</a> | <a href="../itdmstoreelementwithbulk/">ElementWithValues &lt;DataStore&gt;</a>.<a href="../../properties/itdmstoreelementwithbulk-parent/">Parent</a> | <a href="../../collections/freeelementlist-2/">FreeElementList &lt;DataStore&gt;</a>.<a href="../../methods/itdmfreestoreelementlist-add/">Add</a> | <a href="../../collections/freeelementlist-2/">FreeElementList &lt;DataStore&gt;</a>.<a href="../../methods/itdmfreestoreelementlist-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMStoreElement.htm`*
