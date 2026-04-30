---
title: "ITDMTimeDisp.SecondsFrom1904"
description: "Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 1/1/1904."
---

# ITDMTimeDisp.SecondsFrom1904

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: SecondsFrom1904 for UsiTimeDisp

Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 1/1/1904.

## Signature

```python
obj.SecondsFrom1904
```

## Python example

```python
oMyTimeObj = dd.CreateTime(2013,9,13,10,51,44,123,456,789)
dd.MsgBoxDisp("Fractions: " + oMyTimeObj.Fraction + "\r\n" + "Seconds from 0000: " + oMyTimeObj.SecondsFrom0000 + "\r\n" + "Seconds from 1904: " + oMyTimeObj.SecondsFrom1904)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_SecondsFrom1904_ITDMTimeDisp.htm`*
