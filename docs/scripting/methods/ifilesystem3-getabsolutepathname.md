---
title: "IFileSystem3.GetAbsolutePathName"
description: "Returns a unique path."
---

# IFileSystem3.GetAbsolutePathName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetAbsolutePathName for FileSystemObject

Returns a unique path.

## Signature

```python
sGetAbsolutePathName = Object.GetAbsolutePathName(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetAbsolutePath(sPath):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    GetAbsolutePath = fso.GetAbsolutePathName(sPath)

dd.MsgBox(GetAbsolutePath("c:"))  # Returns C:\Program Files\DIAdem
dd.MsgBox(GetAbsolutePath("c:.."))  # Returns C:\Program Files
dd.MsgBox(GetAbsolutePath("c:\"))  # Returns C:\
dd.MsgBox(GetAbsolutePath("c:*.*\test"))  # Returns C:\Program Files\DIAdem\*.*\test
dd.MsgBox(GetAbsolutePath("test"))  # Returns C:\Program Files\DIAdem\test
dd.MsgBox(GetAbsolutePath("c:\..\..\test"))  # Returns C:\test
dd.MsgBox(GetAbsolutePath("C:\Program Files\DIAdem\.."))  # Returns C:\Program Files\
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetAbsolutePathName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
