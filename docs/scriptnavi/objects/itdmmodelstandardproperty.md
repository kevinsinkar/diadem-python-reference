---
title: "ITDMModelStandardProperty"
description: "The ModelStandardProperty object provides the standard property of an entity in the data model of a data store."
---

# ITDMModelStandardProperty

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ModelStandardProperty

The ModelStandardProperty object provides the standard property of an entity in the data model of a data store.

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
oMyFirstModelEntityProperties = oMyDataStoreModel.Entities("MeaQuantity").ModelProperties
for oProperty in oMyFirstModelEntityProperties:
    if oProperty.IsKindOf("ModelEnumerationProperty") :
        print("Enumeration Property: " + oProperty.Name)
    elif oProperty.IsKindOf("ModelStandardProperty") :
        print("Standard Property: " + oProperty.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmmodelstandardproperty-basename/">BaseName</a> | <a href="../../properties/itdmmodelstandardproperty-datatype/">DataType</a> | <a href="../../properties/itdmmodelstandardproperty-maxoccur/">MaxOccur</a> | <a href="../../properties/itdmmodelstandardproperty-minoccur/">MinOccur</a> | <a href="../../properties/itdmmodelstandardproperty-name/">Name</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmmodelstandardproperty-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/modelproperties/">ModelProperties</a>.<a href="../../methods/itdmmodelproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMModelStandardProperty.htm`*
