---
title: "IFileSystem3.CopyFile"
description: "Copies one or more files to a different folder or to another file."
---

# IFileSystem3.CopyFile

!!! abstract "Method &middot; `Scripting.chm`"
    Method: CopyFile for FileSystemObject

Copies one or more files to a different folder or to another file.

## Signature

```python
obj.CopyFile(Source, Destination, [OverWriteFiles])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The CopyFile method aborts as soon as the first error occurs. DIAdem does not undo changes made to the file system before an error occurred.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CopyMyFile(sSource,sTarget,bOverwrite):
    fso = CreateObject("Scripting.FileSystemObject")
    fso.CopyFile(sSource,sTarget,bOverwrite)
CopyMyFile(ProgramDrv + "Examples\Documents\*.tdr", "c:\Temp",True)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_CopyFile_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
