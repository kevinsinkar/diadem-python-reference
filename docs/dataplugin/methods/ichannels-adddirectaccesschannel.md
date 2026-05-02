---
title: "IChannels.AddDirectAccessChannel"
description: "Adds an object to the Channels collection and returns a DirectAccessChannel object."
---

# IChannels.AddDirectAccessChannel

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddDirectAccessChannel for Channels <DataPlugin>

Adds an object to the Channels collection and returns a DirectAccessChannel object.

## Signature

```python
return_value = obj.AddDirectAccessChannel(oDAChn)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
12.06.2004; 1.3452¶
13.06.2004; 1.7834¶
14.06.2004; 2.0034¶
15.06.2004; 1.9996¶
16.06.2004; 1.5649¶
17.06.2004; 1.8957¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.TimeFormat = "DD.MM.YYYY"
File.Formatter.Delimiters = ";"
File.Formatter.Decimalpoint = "."

oMyGrp.Channels.AddDirectAccessChannel(oChn1)
oMyGrp.Channels.AddDirectAccessChannel(oChn2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddDirectAccessChannel_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
