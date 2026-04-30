---
title: "ChnIsolinesCalc"
description: "Calculates contour lines on a surface with a triplet structure."
---

# ChnIsolinesCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnIsolinesCalc

Calculates contour lines on a surface with a triplet structure.

## Signature

```python
dd.ChnIsolinesCalc( X , Y , Z )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The value of the variable <span class="Monospace">HullFactor</span> should not be greater than the value of the variable <a href="../../../varoff/variables/hulltol/">HullTol</a> that specifies the maximum edge length of the hull.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You only can use the <span class="Monospace">D3IsolineBdry</span> variable if the input data have a matrix structure.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem saves the associated contour value in the <span class="Monospace">ResultIsovalue</span> custom property of the respective result channel.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>Z</em></td>
<td>Specifies the data channel containing the z-values.</td></tr>
</table>
</div>

## Python example

```python
dd.D3IsoLineSource ="taken from channel"
dd.D3IsoLineChn ="Grp/Isolines"
dd.D3IsoLineBDryPol ="convex hull"
dd.ChnIsolinesCalc("Grp/Chn1","Grp/Chn2","Grp/Chn3")
```

---

*Source: `ComOff/ChnIsolinesCalc.htm`*
