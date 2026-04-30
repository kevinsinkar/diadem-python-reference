---
title: "IUsiTimeDisp.SecondsFrom0000"
description: "Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 01/01/0000."
---

# IUsiTimeDisp.SecondsFrom0000

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: SecondsFrom0000 for UsiTimeDisp

Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 01/01/0000.

## Signature

```python
obj.SecondsFrom0000
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyTimeObj = CreateTime(2013,9,13,10,51,44,123,456,789)
MsgBoxDisp("Fractions: " + oMyTimeObj.Fraction + vbCrLf + "Seconds from 0000: " + oMyTimeObj.SecondsFrom0000 + vbCrLf + "Seconds from 1904: " + oMyTimeObj.SecondsFrom1904)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_SecondsFrom0000_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
