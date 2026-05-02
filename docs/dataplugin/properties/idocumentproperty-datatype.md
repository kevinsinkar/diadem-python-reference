---
title: "IDocumentProperty.DataType"
description: "Returns the data type of a meta property of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file."
---

# IDocumentProperty.DataType

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: DataType for DocumentProperty <DataPlugin>

Returns the data type of a meta property of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file.

## Signature

```python
obj.DataType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eI32` | 3 | 32-bit integer values |
| `eR64` | 10 | 64-bit real values |
| `eString` | 23 | Text |
| `eTime` | 30 | Time values |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProp in Document.Properties:
    pass
    # select oMyprop.DataType
    # case eI32	sMyPrefix = "i_"
    # case eR64	sMyPrefix = "r_"
    # case eString	sMyPrefix = "s_"
    # case eTime	sMyPrefix = "t_"
    # case Else	sMyPrefix = ""
Root.Properties.Add(sMyPrefixoMyProp.Name, oMyProp.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_DataType_IDocumentProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
