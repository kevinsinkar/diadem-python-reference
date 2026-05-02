---
title: "IUsiTimeDisp.SecondsFrom1904"
description: "Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 1/1/1904."
---

# IUsiTimeDisp.SecondsFrom1904

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: SecondsFrom1904 for UsiTimeDisp

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 1/1/1904.

## Signature

```python
obj.SecondsFrom1904
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyTimeObj = CreateTime(2013,9,13,10,51,44,123,456,789)
MsgBoxDisp("Fractions: " + oMyTimeObj.Fraction + "\r\n" + "Seconds from 0000: " + oMyTimeObj.SecondsFrom0000 + "\r\n" + "Seconds from 1904: " + oMyTimeObj.SecondsFrom1904)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_SecondsFrom1904_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
