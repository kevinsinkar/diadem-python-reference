---
title: "ITDMModelReference"
description: "The ModelReference provides the ModelEntity reference in a data store."
---

# ITDMModelReference

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ModelReference

The ModelReference provides the ModelEntity reference in a data store.

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
oMyEntity = oMyDataStoreModel.Entities(5)
dd.MsgBoxDisp(oMyEntity.ModelReferences(2).Name)
```

## Members

<div markdown="1">
<div class="Properties">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/itdmmodelreference-basename/">BaseName</a> | <a href="../../properties/itdmmodelreference-entitytype/">EntityType</a> | <a href="../../properties/itdmmodelreference-inverse/">Inverse</a> | <a href="../../properties/itdmmodelreference-maxoccur/">MaxOccur</a> | <a href="../../properties/itdmmodelreference-minoccur/">MinOccur</a> | <a href="../../properties/itdmmodelreference-name/">Name</a></p>
</div>
<div class="ReturnFrom">
<h2>Returned From</h2>
<p><a href="./">ModelReference</a>.<a href="../../properties/itdmmodelreference-inverse/">Inverse</a> | <a href="../../collections/modelreferences/">ModelReferences</a>.<a href="../../methods/itdmmodelreferences-item/">Item</a></p>
</div>
</div>
<div class="ReturnFrom">
<h2>Returned From</h2>
<p><a href="./">ModelReference</a>.<a href="../../properties/itdmmodelreference-inverse/">Inverse</a> | <a href="../../collections/modelreferences/">ModelReferences</a>.<a href="../../methods/itdmmodelreferences-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMModelReference.htm`*
