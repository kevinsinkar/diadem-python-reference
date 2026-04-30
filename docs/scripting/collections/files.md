---
title: "Files"
description: "Collection of all File objects. You can use the Files collection to count files or to access individual files."
---

# Files

!!! abstract "Collection &middot; `Scripting.chm`"
    Collection: Files

Collection of all File objects. You can use the Files collection to count files or to access individual files.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateFileList(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    oMyFiles = oMyFolder.Files
    for oMyFile in oMyFiles:
        sOutput = sOutput + oMyFile.Path + VBCrLf
    CreateFileList = sOutput
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifilecollection-count/">Count</a> | <a href="../../properties/ifilecollection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ifolder/">Folder</a>.<a href="../../properties/ifolder-files/">Files</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IFileCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
