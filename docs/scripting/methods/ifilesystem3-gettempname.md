---
title: "IFileSystem3.GetTempName"
description: "Specifies the name of a temporary folder or a temporary file."
---

# IFileSystem3.GetTempName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetTempName for FileSystemObject

Specifies the name of a temporary folder or a temporary file.

## Signature

```python
sGetTempName = Object.GetTempName
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateTempFile():
    fso = CreateObject("Scripting.FileSystemObject")
    TemporaryFolder = 2
    oMyTempFolder = fso.GetSpecialFolder(TemporaryFolder)
    sTempName = fso.GetTempName
    CreateTempFile = oMyTempFolder.CreateTextFile(sTempName)

oMyTempFile = CreateTempFile
oMyTempFile.WriteLine "This is a temporary file!"
oMyTempFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetTempName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
