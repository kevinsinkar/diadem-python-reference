---
title: "IFormatter.ThousandSeparator"
description: "Specifies the thousands separator, which is ignored when values are read in."
---

# IFormatter.ThousandSeparator

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: ThousandSeparator for Formatter

Specifies the thousands separator, which is ignored when values are read in.

## Signature

```python
obj.ThousandSeparator
```

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

*Source: `DataPlugin/Properties/DataPlugin_property_ThousandSeparator_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
