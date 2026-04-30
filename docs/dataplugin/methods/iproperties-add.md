---
title: "IProperties.Add"
description: "Adds an object to the Properties collection and returns a Property object."
---

# IProperties.Add

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Add for Properties <DataPlugin>

Adds an object to the Properties collection and returns a Property object.

## Signature

```python
return_value = obj.Add(sName, Value)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If the specified property exists, the <span class="Monospace">Add</span> method overwrites the value of the property.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.ChannelGroups(1).Properties.Add("Tester","B.Counter")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Add_IProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
