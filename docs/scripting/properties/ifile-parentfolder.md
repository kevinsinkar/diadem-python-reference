---
title: "IFile.ParentFolder"
description: "Returns the Folder object of the superordinate folder for a file. You can use this to access the associated folder of a file."
---

# IFile.ParentFolder

!!! abstract "Property &middot; `Scripting.chm`"
    Property: ParentFolder for File

Returns the Folder object of the superordinate folder for a file. You can use this to access the associated folder of a file.

## Signature

```python
return_value = obj.ParentFolder
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowParentFolder(sFile):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    ShowParentFolder = oMyFile.ParentFolder
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_ParentFolder_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
