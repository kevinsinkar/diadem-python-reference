---
title: "IProcessedChannel.AddCharacteristics"
description: "Specifies the characteristic values of a channel which combines the values from other channels ( ChannelsToProcess )."
---

# IProcessedChannel.AddCharacteristics

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddCharacteristics for ProcessedChannel

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the characteristic values of a channel which combines the values from other channels ( ChannelsToProcess ).

## Signature

```python
obj.AddCharacteristics(Minimum, Maximum, Monotony, NoValueKey)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eMonotonyUnknown` | 1 | Not calculated |
| `eMonotonyIncreasing` | 2 | Increasing |
| `eMonotonyDecreasing` | 3 | Decreasing |
| `eMonotonyNo` | 4 | Not monotone |
| `eNoValueKeyNotCalculated` | 1 | Not calculated |
| `eNoValueKeyYes` | 2 | Yes |
| `eNoValueKeyNo` | 3 | No |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for Channel in ChannelGroup.Channels:
    if Channel.IsKindOf(eDirectAccess) and (Channel.DataType == eR64):
        ProcessedChn.Channels.Add(Channel)
ProcessedChn.AddCharacteristics(0,1000,eMonotonyUnknown,eNoValueKyNotCalculated)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddCharacteristics_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
