---
title: "IFormatter.NoValueSign"
description: "Specifies the NoValue character used in the file."
---

# IFormatter.NoValueSign

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: NoValueSign for Formatter

Specifies the NoValue character used in the file.

## Signature

```python
obj.NoValueSign
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
15.12.1998 12:00:00; 2.84529E-04¶
15.01.1999 12:00:00; 1.05914E-04¶
14.02.1999 12:00:00; 2.84483E-04¶
16.03.1999 12:00:00; NV¶
16.04.1999 12:00:00; 5.47222E-04¶
16.05.1999 12:00:00; 0.00010¶
16.06.1999 12:00:00; 0.00012¶
16.07.1999 12:00:00; 0.00015¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.Delimiters = ";"
File.Formatter.Timeformat = "DD.MM.YYYY hh:mm:ss"
File.Formatter.DecimalPoint = "."
File.Formatter.NoValueSign = "NV"
File.Formatter.ExponentSeparator = "E"

oGrp.Channels.AddDirectAccessChannel(oChn)
oChn = oBlock.Channels.Add("YShift", eR64)
oGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_NoValueSign_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
