---
title: "IChannelsToProcess.Add"
description: "Adds an object to the ChannelsToProcess collection and returns a Channel object."
---

# IChannelsToProcess.Add

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Add for ChannelsToProcess

Adds an object to the ChannelsToProcess collection and returns a Channel object.

## Signature

```python
return_value = obj.Add(oChannel)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oStringBlock  = File.GetStringBlock()
oDateChn      = oStringBlock.Channels.Add("Date", eTime)
oTimeChn      = oStringBlock.Channels.Add("Time", eTime)
oChannelGroup = Root.ChannelGroups.Add("Measurements")
oProcessedChn = oChannelGroup.Channels.AddProcessedChannel("MyChannel",eTime,eAddProcessor)
oProcessedChn.Channels.Add(oDateChn)
oProcessedChn.Channels.Add(oTimeChn)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Add_IChannelsToProcess.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
