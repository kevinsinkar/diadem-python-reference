---
title: "IStringChannelFormatter"
description: "The StringChannelFormatter object contains information about how the values of a channel are represented in the text file."
---

# IStringChannelFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: StringChannelFormatter

The StringChannelFormatter object contains information about how the values of a channel are represented in the text file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in oBlock.Channels:
    if (oMyChn.Formatter.IsKindOf(eStringBlock)):
        oMyChn.Properties.Add("DataType", oMyChn.Formatter.DataType)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/istringchannelformatter-block/">Block</a> | <a href="../../properties/istringchannelformatter-datatype/">DataType</a> | <a href="../../properties/istringchannelformatter-decimalpoint/">DecimalPoint</a> | <a href="../../properties/istringchannelformatter-novaluesign/">NoValueSign</a> | <a href="../../properties/istringchannelformatter-thousandseparator/">ThousandSeparator</a> | <a href="../../properties/istringchannelformatter-timeformat/">TimeFormat</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/istringchannelformatter-iskindof/">IsKindOf</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IStringChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
