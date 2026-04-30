---
title: "IToVideoInt.SetVideo"
description: "Specifies whether DIAdem uses a video file or a video channel in a video in DIAdem VIEW and specifies the name of the video file or the channel reference of the"
---

# IToVideoInt.SetVideo

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: SetVideo for Video

Specifies whether DIAdem uses a video file or a video channel in a video in DIAdem VIEW and specifies the name of the video file or the channel reference of the video channel. Use the FileName for Video property to specify the name of the video. Use the VideoSourceMode for Video property to specify whether DIAdem uses a video file or a video channel.

## Signature

```python
obj.SetVideo(VideoSourceMode, FilenameOrVideoChannelName)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eVideoFile` | 0 | Video file |
| `eVideoChannel` | 1 | Video channel |

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Video"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.SetVideo(dd.eVideoFile, dd.ProgramDrv + "Examples\\Documents\\Safetytest01.wmv")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_SetVideo_IToVideoInt.htm`*
