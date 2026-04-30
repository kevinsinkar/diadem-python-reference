---
title: "IFolder.IsRootFolder"
description: "Checks whether a folder is the root folder."
---

# IFolder.IsRootFolder

!!! abstract "Property &middot; `Scripting.chm`"
    Property: IsRootFolder for Folder

Checks whether a folder is the root folder.

## Signature

```python
obj.IsRootFolder
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CountLevelDepth(sPath):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sPath)
    iCount = 0
    while not oMyFolder.IsRootFolder:
        oMyFolder = oMyFolder.ParentFolder
        iCount = iCount + 1
    CountLevelDepth = iCount
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_IsRootFolder_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
