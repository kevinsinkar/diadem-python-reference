---
title: "IDataPlugin.CurrentScriptName"
description: "Specifies the name of the script file which belongs to the currently executed DataPlugin."
---

# IDataPlugin.CurrentScriptName

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: CurrentScriptName for DataPlugin

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the name of the script file which belongs to the currently executed DataPlugin.

## Signature

```python
obj.CurrentScriptName
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("ScriptName",CurrentScriptName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_CurrentScriptName_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
