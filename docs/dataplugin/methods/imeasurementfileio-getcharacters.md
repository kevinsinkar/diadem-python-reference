---
title: "IMeasurementFileIO.GetCharacters"
description: "Reads a specific number of characters from the file. The method returns all characters, including delimiters and end of line characters."
---

# IMeasurementFileIO.GetCharacters

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetCharacters for File

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Reads a specific number of characters from the file. The method returns all characters, including delimiters and end of line characters.

## Signature

```python
sGetCharacters = Object.GetCharacters(Number)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  If <span class="Monospace">GetCharacters</span> finds the character "\0" before it has read the specified number of characters, <span class="Monospace">GetCharacters</span> returns only the characters it has read up to that point.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
BytesToRead = 1000
if (BytesToRead > File.Size):
    BytesToRead = File.Size
ByteStream = File.GetCharacters(BytesToRead))
if (0 < Instr(ByteStream,"\n")):
    File.Formatter.LineFeeds = "\n"
elif (0 < Instr(ByteStream,"\r")):
    File.Formatter.LineFeeds = "\r"
elif (0 < Instr(ByteStream,"\n")):
    File.Formatter.LineFeeds = "\n"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetCharacters_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
