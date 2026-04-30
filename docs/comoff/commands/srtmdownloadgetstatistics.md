---
title: "SRTMDownloadGetStatistics"
description: "Specifies various statistical values on the SRTM data within the specified latitude-longitude range. The SRTM data contains a high-resolution digital terrain mo"
---

# SRTMDownloadGetStatistics

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SRTMDownloadGetStatistics

Specifies various statistical values on the SRTM data within the specified latitude-longitude range. The SRTM data contains a high-resolution digital terrain model of the earth surface with the elevation value for nearly every position on the earth.

## Signature

```python
dd.SRTMDownloadGetStatistics(SRTMLowerLatitudeBound, SRTMUpperLatitudeBound, SRTMLowerLongitudeBound, SRTMUpperLongitudeBound, SRTMTilesAvailable, SRTMTilesToDownload, SRTMTilesMissing, SRTMMegaBytesOnDisk, SRTMMegaBytesToDownload, SRTMAreaNotSupported)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SRTMLowerLatitudeBound</td>
<td>Specifies the lower latitude limit.<div id="exp_SRTMLowerLatitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMUpperLatitudeBound</td>
<td>Specifies the upper latitude limit.<div id="exp_SRTMUpperLatitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMLowerLongitudeBound</td>
<td>Specifies the lower longitude limit.<div id="exp_SRTMLowerLongitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMUpperLongitudeBound</td>
<td>Specifies the upper longitude limit.<div id="exp_SRTMUpperLongitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMTilesAvailable</td>
<td>Receives the information on how many tiles are available online within the specified area.<div id="exp_SRTMTilesAvailable">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMTilesToDownload</td>
<td>Receives the information on how many tiles within the specified area DIAdem still must download.<div id="exp_SRTMTilesToDownload">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMTilesMissing</td>
<td>Receives the information on how many tiles are not available online within the specified area.<div id="exp_SRTMTilesMissing">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMMegaBytesOnDisk</td>
<td>Receives the information on how many MB on the hard disk are occupied by the downloaded area.<div id="exp_SRTMMegaBytesOnDisk">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMMegaBytesToDownload</td>
<td>Receives the information on how many MB are necessary to download the tiles of the specified area.<div id="exp_SRTMMegaBytesToDownload">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMAreaNotSupported</td>
<td>Receives the information on whether SRTM data is available for the specified area.<div id="exp_SRTMAreaNotSupported">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/SRTMDownloadGetStatistics.htm`*
