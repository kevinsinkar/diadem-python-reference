---
title: "ITextStream.Read"
description: "Reads one or more characters from a TextStream file."
---

# ITextStream.Read

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Read for TextStream

Reads one or more characters from a TextStream file.

## Signature

```python
sRead = Object.Read(Characters)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadCharacters(sFile):
    ForReading = 1; ForWriting = 2
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile= fso.OpenTextFile(sFile, ForWriting, True)
    oMyFile.Write "This is a text"
    oMyFile = fso.OpenTextFile(sFile, ForReading)
    ReadCharacters = oMyFile.Read(4)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Read_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
