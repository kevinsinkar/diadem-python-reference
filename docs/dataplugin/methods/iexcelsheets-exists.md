---
title: "IExcelSheets.Exists"
description: "Checks whether a Sheet object with a specific name or index exists."
---

# IExcelSheets.Exists

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Exists for Sheets

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Checks whether a Sheet object with a specific name or index exists.

## Signature

```python
bExists = Object.Exists(NameOrIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if Workbook.Sheets.Exists("AB_2010"):
    Root.ChannelGroups.Add("AB_2010")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Exists_IExcelSheets.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
