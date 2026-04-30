---
title: "ISUSIElement"
description: "The Element object provides a single element of the search results or of the file browser in a DataFinder. The elements can be files, groups, or channels."
---

# ISUSIElement

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Element <DataFinder>

The Element object provides a single element of the search results or of the file browser in a DataFinder. The elements can be files, groups, or channels.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Depending on whether an element of the search results is a file (<a href="../isusiroot/">Root</a>), a group (<a href="../isusichannelgroup/">Channelgroup</a>) or a channel (<a href="../isusichannel/">Channel</a>), the <span class="Monospace">Element</span> object has additional properties. Use the <a href="../../methods/isusielement-iskindof/">IsKindOf</a> method to determine the type of an element of the search results.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Working with the Elements Collection and the Element Object</a> for general information on working with the elements.</td></tr></table>
</div>

## Python example

```python
oMyResultsList = dd.Navigator.Display.CurrDataFinder.ResultsList
for Element in oMyResultsList.Elements:
    if Element.IsKindOf(dd.eSearchChannel) :
        dd.Navigator.LoadData(Element,"Load")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/isusielement-name/">Name</a> | <a href="../../properties/isusielement-properties/">Properties</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/isusielement-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavidatafinderbrowser/">Browser &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderbrowser-focusedelement/">FocusedElement</a> | <a href="../idatafindercell/">Cell &lt;DataFinder&gt;</a>.<a href="../../properties/idatafindercell-element/">Element</a> | <a href="../../collections/elementlist/">ElementList &lt;DataFinder&gt;</a>.<a href="../../methods/isusielements-item/">Item</a> | <a href="../../collections/elementsselection/">ElementsSelection &lt;DataFinder&gt;</a>.<a href="../../methods/idatafinderresultsdisplayelementsselection-item/">Item</a> | <a href="../../collections/freeelementlist/">FreeElementList &lt;DataFinder&gt;</a>.<a href="../../methods/itdmfreedatafinderelementlist-add/">Add</a> | <a href="../../collections/freeelementlist/">FreeElementList &lt;DataFinder&gt;</a>.<a href="../../methods/itdmfreedatafinderelementlist-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ISUSIElement.htm`*
