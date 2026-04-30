---
title: "IChannel.AddCharacteristics"
description: "Specifies the characteristic values of a channel."
---

# IChannel.AddCharacteristics

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddCharacteristics for Channel <DataPlugin>

Specifies the characteristic values of a channel.

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
for i in range(1, 100 + 1):
    oMyChn.Values(i) = cdbl(i/100000)
oMyChn.AddCharacteristics(1/100000,1/1000,eMonotonyIncreasing, eNoValueKeyNo)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddCharacteristics_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
