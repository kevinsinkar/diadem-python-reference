---
title: "IToVideoInt"
description: "The Video object provides access to a video in DIAdem VIEW. You use the Video object to specify the properties of the video to be displayed."
---

# IToVideoInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Video

The Video object provides access to a video in DIAdem VIEW. You use the Video object to specify the properties of the video to be displayed.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Video"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.FileName = dd.ProgramDrv + "\\Examples\\Documents\\Plate.avi"
oMyObj.FrameRate = 50
oMyObj.Sound = True
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itovideoint-area/">Area</a> | <a href="../../properties/itovideoint-channelname/">ChannelName</a> | <a href="../../properties/itovideoint-cursorreference/">CursorReference</a> | <a href="../../properties/itovideoint-filename/">FileName</a> | <a href="../../properties/itovideoint-framerate/">FrameRate</a> | <a href="../../properties/itovideoint-keepratio/">KeepRatio</a> | <a href="../../properties/itovideoint-noofframes/">NoOfFrames</a> | <a href="../../properties/itovideoint-overlayobjects/">OverlayObjects</a> | <a href="../../properties/itovideoint-sound/">Sound</a> | <a href="../../properties/itovideoint-starttime/">StartTime</a> | <a href="../../properties/itovideoint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itovideoint-transparency/">Transparency</a> | <a href="../../properties/itovideoint-videosourcemode/">VideoSourceMode</a> | <a href="../../properties/itovideoint-xbegin/">XBegin</a> | <a href="../../properties/itovideoint-xend/">XEnd</a> | <a href="../../properties/itovideoint-ybegin/">YBegin</a> | <a href="../../properties/itovideoint-yend/">YEnd</a> | <a href="../../properties/itovideoint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itovideoint-iszoomed/">IsZoomed</a> | <a href="../../methods/itovideoint-setvideo/">SetVideo</a> | <a href="../../methods/itovideoint-showvideodlg/">ShowVideoDlg</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">3D Interpolation</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Recording Video and Measurement Data</a> | <a href="#" data-unresolved="1">Synchronizing Maps, Videos, and Measurement Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToVideoInt.htm`*
