---
title: "IChannels.Add"
description: "Adds an object to the Channels collection and returns a Channel object."
---

# IChannels.Add

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Add for Channels <DataPlugin>

Adds an object to the Channels collection and returns a Channel object.

## Signature

```python
return_value = obj.Add(sName, eDataType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The channel name must be unique and must not include special characters.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eI16` | 2 | 16-bit integer values |
| `eI32` | 3 | 32-bit integer values |
| `eR32` | 9 | 32-bit real values |
| `eR64` | 10 | 64-bit real values |
| `eString` | 23 | Text |
| `eEnum` | 24 | Enumeration |
| `eTime` | 30 | Time values |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python

```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Add_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
