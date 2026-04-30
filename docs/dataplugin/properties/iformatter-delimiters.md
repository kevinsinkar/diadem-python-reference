---
title: "IFormatter.Delimiters"
description: "Specifies the characters that separate values or text in the file."
---

# IFormatter.Delimiters

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Delimiters for Formatter

Specifies the characters that separate values or text in the file.

## Signature

```python
obj.Delimiters
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The specified characters are not a string; they are a list of single characters.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
XAxis; 1.000.000; 2.000; 301¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds = vbNewLine
File.Formatter.Delimiters = ";"
File.Formatter.ThousandSeparator = "."
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Delimiters_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
