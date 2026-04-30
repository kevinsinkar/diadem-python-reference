---
title: "IDirectAccessChannel.AddCharacteristics"
description: "Specifies the characteristic values of a DirectAccessChannel."
---

# IDirectAccessChannel.AddCharacteristics

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddCharacteristics for DirectAccessChannel

Specifies the characteristic values of a DirectAccessChannel.

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
File.GetNextLine

oChn.AddCharacteristics(rMin,rMax,eMonotonyUnknown,eNovalueKeyNotCalculated)
oMyGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddCharacteristics_IDirectAccessChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
