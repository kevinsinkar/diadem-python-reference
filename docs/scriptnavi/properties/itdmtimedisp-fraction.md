---
title: "ITDMTimeDisp.Fraction"
description: "Specifies in an USITimeDisp type object the fractions of a second with an accuracy of nanoseconds."
---

# ITDMTimeDisp.Fraction

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Fraction for UsiTimeDisp

Specifies in an USITimeDisp type object the fractions of a second with an accuracy of nanoseconds.

## Signature

```python
obj.Fraction
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <span class="Monospace">Fraction</span> property returns a value smaller than or equal zero. The <a href="../itdmtimedisp-nanosecond/">Nanosecond</a> property returns the number of nanoseconds.</td></tr></table>
</div>

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

*Source: `ScriptNavi/properties/navigator_property_Fraction_ITDMTimeDisp.htm`*
