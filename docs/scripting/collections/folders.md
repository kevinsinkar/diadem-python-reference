---
title: "Folders"
description: "Collection of all Folder objects. You can use the Folder collection to count folders or to access individual folders."
---

# Folders

!!! abstract "Collection &middot; `Scripting.chm`"
    Collection: Folders

Collection of all Folder objects. You can use the Folder collection to count folders or to access individual folders.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateFolderList(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    oMySubFolders = oMyFolder.SubFolders
    for oMySubFolder in oMySubFolders:
        sOutput = sOutput + oMySubFolder.Path + VbCrLf
        sOutput = sOutput + CreateFolderList(oMySubFolder.Path)
    CreateFolderList = sOutput
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifoldercollection-count/">Count</a> | <a href="../../properties/ifoldercollection-item/">Item</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ifoldercollection-add/">Add</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ifolder/">Folder</a>.<a href="../../properties/ifolder-subfolders/">SubFolders</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IFolderCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
