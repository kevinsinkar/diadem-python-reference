---
title: "IBinaryChannelFormatter"
description: "The BinaryChannelFormatter object contains information about how the values of a channel are represented in the binary file."
---

# IBinaryChannelFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: BinaryChannelFormatter

The BinaryChannelFormatter object contains information about how the values of a channel are represented in the binary file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in oBlock.Channels:
    if (oMyChn.Formatter.IsKindOf(eBinaryBlock)):
        oMyChn.Properties.Add("DataType", oMyChn.Formatter.DataType)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ibinarychannelformatter-bitmask/">BitMask</a> | <a href="../../properties/ibinarychannelformatter-block/">Block</a> | <a href="../../properties/ibinarychannelformatter-byteorder/">ByteOrder</a> | <a href="../../properties/ibinarychannelformatter-datatype/">DataType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ibinarychannelformatter-iskindof/">IsKindOf</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IBinaryChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
