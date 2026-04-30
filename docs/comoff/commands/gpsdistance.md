---
title: "GPSDistance"
description: "Calculates the shortest distance and the angle from the earth’s center between two coordinates taking the ellipsoidal shape of the Earth into account."
---

# GPSDistance

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GPSDistance

Calculates the shortest distance and the angle from the earth’s center between two coordinates taking the ellipsoidal shape of the Earth into account.

## Signature

```python
dd.GPSDistance(Latitude1, Longitude1, Latitude2, Longitude2, EllipsoidGeometryType, ResultDistance, ResultAngle)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Latitude1</td>
<td>Specifies the latitude of the first coordinate.<div id="exp_Latitude1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">Longitude1</td>
<td>Specifies the longitude of the first coordinate.<div id="exp_Longitude1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">Latitude2</td>
<td>Specifies the latitude of the second coordinate.<div id="exp_Latitude2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">Longitude2</td>
<td>Specifies the longitude of the second coordinate.<div id="exp_Longitude2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">EllipsoidGeometryType</td>
<td>Specifies whether DIAdem assumes that the Earth is a sphere or ellipsoid according to the 1984 World Geodetic System (WGS 84).<div id="exp_EllipsoidGeometryType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"eMeanRadius"</pre></donottranslate></td>
<td>Geometry without consideration of the ellipsoidal shape</td></tr>
<tr><td width="150"><donottranslate><pre>"eWGS84"</pre></donottranslate></td>
<td>Geometry according to World Geodetic System 1984 (WGS 84)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ResultDistance</td>
<td>Receives the distance in m.<div id="exp_ResultDistance">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ResultAngle</td>
<td>Receives the angle in degrees.<div id="exp_ResultAngle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/GPSDistance.htm`*
