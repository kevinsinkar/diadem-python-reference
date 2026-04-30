---
title: "ITDMTimeDisp.SecondsFrom0000"
description: "Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 01/01/0000."
---

# ITDMTimeDisp.SecondsFrom0000

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: SecondsFrom0000 for UsiTimeDisp

Specifies in a USITimeDisp type object the seconds since 00:00:00 o'clock on 01/01/0000.

## Signature

```python
obj.SecondsFrom0000
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong> If the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution has</a> the value <span class="Monospace">FALSE</span> , the sum of the values <span class="style1">of</span> <span class="Monospace">SecondsFrom0000</span> and <a href="../itdmtimedisp-fraction/">Fraction</a> corresponds to the double value in DIAdem time format.<br attr="ext"/>If the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a> has the value <span class="Monospace">FALSE</span>, the DIAdem time format can only record fractions of a second with a maximum of 4 digits.</td></tr></table>
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

*Source: `ScriptNavi/properties/navigator_property_SecondsFrom0000_ITDMTimeDisp.htm`*
