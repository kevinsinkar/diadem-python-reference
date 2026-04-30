---
title: "IToVideoInt.FileName"
description: "Specifies the name of a video in DIAdem VIEW. If you have assigned the eVideoChannel value to the VideoSourceMode property, the property is read-only and contai"
---

# IToVideoInt.FileName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: FileName for Video

Specifies the name of a video in DIAdem VIEW. If you have assigned the eVideoChannel value to the VideoSourceMode property, the property is read-only and contains the video name with an absolute path, even if the video channel contains a relative path. If you have assigned the eVideoFile value to the VideoSourceMode property, the property can be read and written and contains the video name with or without a path. Use the SetVideo for Video method to specify whether DIAdem uses a video file or a video channel and to specify the name with path of the video file or the channel reference of the video channel.

## Signature

```python
obj.FileName
```

## Python example

```python
oMyArea = dd.View.ActiveSheet.ActiveArea.SplitBottom("NewVideo", 0.5)
oMyArea.DisplayObjType = "Video"
oMyObj = oMyArea.DisplayObj
oMyObj.FileName = dd.ProgramDrv  + "Examples\\Documents\\Austin_Drive.wmv"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_FileName_IToVideoInt.htm`*
