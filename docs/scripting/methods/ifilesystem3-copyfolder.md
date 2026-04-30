---
title: "IFileSystem3.CopyFolder"
description: "Copies a folder into another folder."
---

# IFileSystem3.CopyFolder

!!! abstract "Method &middot; `Scripting.chm`"
    Method: CopyFolder for FileSystemObject

Copies a folder into another folder.

## Signature

```python
obj.CopyFolder(Source, Destination, [OverWriteFiles])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The CopyFolder method aborts as soon as the first error occurs. DIAdem does not undo changes made to the file system before an error occurred.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CopyEntireFolder(sSource,sTarget,bOverwrite):
    fso = CreateObject("Scripting.FileSystemObject")
    fso.CopyFolder(sSource,sTarget,bOverwrite)
CopyEntireFolder(ProgramDrv + "Examples\Docume*", "c:\Temp",True)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_CopyFolder_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
