---
title: "IFileSystem3.OpenTextFile"
description: "Creates and opens a file for reading, writing, or appending and returns a TextStream object."
---

# IFileSystem3.OpenTextFile

!!! abstract "Method &middot; `Scripting.chm`"
    Method: OpenTextFile for FileSystemObject

Creates and opens a file for reading, writing, or appending and returns a TextStream object.

## Signature

```python
return_value = obj.OpenTextFile(FileName, [IOMode], [Create], [Format])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadWriteAppend(sFile):
    ForReading = 1; ForWriting = 2; ForAppending = 8
    TristateUseDefault = -2; TristateTrue = -1; TristateFalse = 0
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    # Open the file for output
    oMyFile = fso.OpenTextFile(sFile, ForWriting, True)
    # Write to the file.
    oMyFile.WriteLine "This is the first line"
    oMyFile.Close

    # Open the file for appending
    oMyFile = fso.OpenTextFile(sFile, ForAppending, True)
    # Write to the file.
    oMyFile.WriteLine "This is the second line"
    oMyFile.Close

    # Open the file for input
    oMyFile = fso.OpenTextFile(sFile, ForReading)
    # Read from the file
    dd.MsgBox(oMyFile.ReadAll)
    oMyFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_OpenTextFile_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
