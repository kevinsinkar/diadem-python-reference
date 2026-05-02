---
title: "Elements"
description: "Collection of all Element objects. These objects contain information about the currently edited data store. The elements from this collection might be ChannelGr"
---

# Elements

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: Elements <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Collection of all Element objects. These objects contain information about the currently edited data store. The elements from this collection might be ChannelGroup or Channel types.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If the data store currently processed by the DataFinder contains several channels with the same name, the DataPlugIn only loads the first of those channels with the file loader, for example <span class="Monospace">DataPlugin(CSV)</span>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadStore(FromStore):
    FindAndCreateGroups(FromStore.Children)

def FindAndCreateGroups(StoreElements):
    for StoreElement in StoreElements:
        if StoreElement.IsKindOf(eStoreChannelGroup):
            TDMGroup = Root.ChannelGroups.Add(StoreElement.Name)
            TDMGroup.Properties.AddProperties(StoreElement.Properties)
        else:
            FindAndCreateGroups(StoreElement.Children)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iusielements-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iusielements-item/">Item</a> | <a href="../../methods/iusielements-remove/">Remove</a> | <a href="../../methods/iusielements-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IUSIElements.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
