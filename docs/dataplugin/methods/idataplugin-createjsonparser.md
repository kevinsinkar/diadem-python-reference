---
title: "IDataPlugin.CreateJsonParser"
description: "Creates a JsonParser object with methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object or a VBS ar"
---

# IDataPlugin.CreateJsonParser

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: CreateJsonParser for DataPlugin

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Creates a JsonParser object with methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object or a VBS array , or vice versa.

## Signature

```python
return_value = obj.CreateJsonParser
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oJsonParser = CreateJsonParser()
sJsonString = oJsonParser.ReadFile("c:\JsonObject.json")
oJsonParser.Deserialize(sJsonString, oVbsVariant)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_CreateJsonParser_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
