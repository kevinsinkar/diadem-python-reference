---
title: "IFolderCollection.Add"
description: "DIAdem adds a new folder object to the folders collection by creating a new folder."
---

# IFolderCollection.Add

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Add for Folders

DIAdem adds a new folder object to the folders collection by creating a new folder.

## Signature

```python
return_value = obj.Add(Name)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def AddNewFolder(sPath, sFolderName):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sPath)
    oMySubFolders = oMyFolder.SubFolders
    if sFolderName != "":
        oNewFolder = oMySubFolders.Add(sFolderName)
    else:
        oNewFolder = oMySubFolders.Add("New Folder")
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Add_IFolderCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
