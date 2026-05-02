---
title: "IFormatter.CommentSign"
description: "Specifies the characters that mark comment lines in the file. These characters must be at the start of the line."
---

# IFormatter.CommentSign

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: CommentSign for Formatter

Specifies the characters that mark comment lines in the file. These characters must be at the start of the line.

## Signature

```python
obj.CommentSign
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong> When the file is read in, the characters are case sensitive. For example, if you enter the identifier <span class="Monospace">REM</span>, a line marked <span class="Monospace">Rem</span> is not skipped when being read.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyMeasurementData¶
rem generation specification for implicit channel¶
XAxis; 1.000.000; 2.000; 301¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.Delimiters = ";"
File.Formatter.CommentSign= "rem"
File.SkipLine()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_CommentSign_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
