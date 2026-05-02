---
title: "IFolder.CreateTextFile"
description: "Creates a file in a folder and returns the associated TextStream object."
---

# IFolder.CreateTextFile

!!! abstract "Method &middot; `Scripting.chm`"
    Method: CreateTextFile for Folder

Creates a file in a folder and returns the associated TextStream object.

## Signature

```python
return_value = obj.CreateTextFile(FileName, [Overwrite], [Unicode])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateMyTxtFile(sFolder,sFile,sText):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    oMyFile = oMyFolder.CreateTextFile(sFile, True)
    oMyFile.WriteLine(sText)
    oMyFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_CreateTextFile_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
