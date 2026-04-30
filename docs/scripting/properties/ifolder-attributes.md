---
title: "IFolder.Attributes"
description: "Checks the attributes of a folder."
---

# IFolder.Attributes

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Attributes for Folder

Checks the attributes of a folder.

## Signature

```python
obj.Attributes
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def MakeWritable(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    if oMyFolder.Attributes and 1:
        oMyFolder.Attributes = oMyFolder.Attributes - 1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Attributes_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
