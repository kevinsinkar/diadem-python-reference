---
title: "IUsiTimeDisp.Fraction"
description: "Specifies in an USITimeDisp type object the fractions of a second with an accuracy of nanoseconds."
---

# IUsiTimeDisp.Fraction

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Fraction for UsiTimeDisp

Specifies in an USITimeDisp type object the fractions of a second with an accuracy of nanoseconds.

## Signature

```python
obj.Fraction
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <span class="Monospace">Fraction</span> property returns a value smaller than or equal zero. The property <a href="../iusitimedisp-nanosecond/">Nanosecond</a> returns the number of nanoseconds.</td></tr></table>
</div>

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

*Source: `DataPlugin/Properties/DataPlugin_property_Fraction_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
