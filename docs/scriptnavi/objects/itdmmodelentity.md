---
title: "ITDMModelEntity"
description: "The Entity object provides an entity of the data model."
---

# ITDMModelEntity

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ModelEntity

The Entity object provides an entity of the data model.

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyModel = oMyDataStore.Model
oMyEntity = oMyModel.Entities(1)
dd.MsgBoxDisp(oMyEntity.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmmodelentity-modelproperties/">ModelProperties</a> | <a href="../../properties/itdmmodelentity-modelreferences/">ModelReferences</a> | <a href="../../properties/itdmmodelentity-name/">Name</a> | <a href="../../properties/itdmmodelentity-subtypes/">SubTypes</a> | <a href="../../properties/itdmmodelentity-supertype/">SuperType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmmodelentity-isbasetype/">IsBaseType</a> | <a href="../../methods/itdmmodelentity-iskindof/">IsKindOf</a> | <a href="../../methods/itdmmodelentity-isvalid/">IsValid</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmbrowseentity/">BrowseEntity</a>.<a href="../../properties/itdmbrowseentity-entitytype/">EntityType</a> | <a href="../../collections/modelentities/">ModelEntities</a>.<a href="../../methods/itdmmodelentities-item/">Item</a> | <a href="./">ModelEntity</a>.<a href="../../properties/itdmmodelentity-supertype/">SuperType</a> | <a href="../itdmmodelreference/">ModelReference</a>.<a href="../../properties/itdmmodelreference-entitytype/">EntityType</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMModelEntity.htm`*
