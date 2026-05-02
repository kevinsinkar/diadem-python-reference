---
title: "IFileSystem3.FileExists"
description: "Checks whether a file exists."
---

# IFileSystem3.FileExists

!!! abstract "Method &middot; `Scripting.chm`"
    Method: FileExists for FileSystemObject

Checks whether a file exists.

## Signature

```python
bFileExists = Object.FileExists(FileSpec)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FileStatus(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    if (fso.FileExists(sFile)):
        sOutput = sFile + " exists."
    else:
        sOutput = sFile + " doesn't exist."
    FileStatus = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_FileExists_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
