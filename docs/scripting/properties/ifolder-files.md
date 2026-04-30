---
title: "IFolder.Files"
description: "Returns the file collection for a Folder object. You can use this to access the files in a folder."
---

# IFolder.Files

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Files for Folder

Returns the file collection for a Folder object. You can use this to access the files in a folder.

## Signature

```python
return_value = obj.Files
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CountFiles(folderspec):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(folderspec)
    oMyFiles = oMyFolder.Files
    CountFiles = "Number of Files: " + oMyFiles.Count
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Files_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
