---
title: "IExcelFileIO.Formatter"
description: "Returns the Formatter object that contains information about the format of the workbook that the DataPlugin is currently processing."
---

# IExcelFileIO.Formatter

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Formatter for Workbook

Returns the Formatter object that contains information about the format of the workbook that the DataPlugin is currently processing.

## Signature

```python
return_value = obj.Formatter
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
0,3	958,4	29,8¶
0,4	1137,7	36,4¶
0,5	#NV	44,1¶
0,6	1474,6	#NV¶
0,7	#NV	68,4¶

Workbook.Formatter.NoValueSign = "#NV"

for iCol in range(1, 3 + 1):
    oChannel= oBlock.Channels.Add("Channel")
    oGroup.Channels.AddDirectAccessChannel(oChannel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Formatter_IExcelFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
