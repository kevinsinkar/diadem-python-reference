---
title: "IProperties.RemoveAll"
description: "Deletes all elements from the Properties collection."
---

# IProperties.RemoveAll

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: RemoveAll for Properties <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Deletes all elements from the Properties collection.

## Signature

```python
obj.RemoveAll
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.ChannelGroups(1).Properties.RemoveAll
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_RemoveAll_IProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
