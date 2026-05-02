---
title: "ITextStream.Skip"
description: "Skips one or more characters when reading a TextStream file."
---

# ITextStream.Skip

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Skip for TextStream

Skips one or more characters when reading a TextStream file.

## Signature

```python
obj.Skip(Characters)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def SkipCharacters(sFile):
    ForReading = 1; ForWriting = 2
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile= fso.OpenTextFile(sFile, ForWriting, True)
    oMyFile.Write "This is a text"
    oMyFile = fso.OpenTextFile(sFile, ForReading)
    oMyFile.Skip(10)
    SkipCharacters = oMyFile.ReadLine
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Skip_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
