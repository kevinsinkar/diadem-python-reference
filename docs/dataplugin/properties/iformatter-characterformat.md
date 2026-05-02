---
title: "IFormatter.CharacterFormat"
description: "Specifies the coding for interpreting the strings in the file."
---

# IFormatter.CharacterFormat

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: CharacterFormat for Formatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the coding for interpreting the strings in the file.

## Signature

```python
obj.CharacterFormat
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify the coding, it is specified automatically. The first two bytes in the file are checked. If the first two bytes contain <span class="Monospace">0xFEFF</span>, this indicates UTF16 coding.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eUTF16` | 0 | 16-bit characters that allow Asian characters, for example. |
| `eANSI` | 1 | Extended ASCII character set (8-bit). |
| `eSJIS` | 3 | Shift-JIS character set for the Japanese language. |
| `eUTF8` | 4 | 8-bit character set commonly used for encoding English texts. |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds = "\n"
File.Formatter.Delimiters = ";"
File.Formatter.CharacterFormat = eUTF16
oMyGrp.Channels.AddDirectAccessChannel(Channel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_CharacterFormat_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
