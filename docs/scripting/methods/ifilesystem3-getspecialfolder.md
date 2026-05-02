---
title: "IFileSystem3.GetSpecialFolder"
description: "Returns a particular folder."
---

# IFileSystem3.GetSpecialFolder

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetSpecialFolder for FileSystemObject

Returns a particular folder.

## Signature

```python
return_value = obj.GetSpecialFolder(SpecialFolder)
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

*Source: `Scripting/methods/Scripting_method_GetSpecialFolder_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
