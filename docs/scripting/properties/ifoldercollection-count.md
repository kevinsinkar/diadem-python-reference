---
title: "IFolderCollection.Count"
description: "Returns the number of folders."
---

# IFolderCollection.Count

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Count for Folders

Returns the number of folders.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CountFolders(sFolderSpec):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolderSpec)
    oMySubFolders = oMyFolder.SubFolders
    CountFolders = "Number of folders: " + oMySubFolders.Count
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Count_IFolderCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
