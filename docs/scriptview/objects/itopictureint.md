---
title: "IToPictureInt"
description: "The Picture object provides access to a graphic in DIAdem VIEW. You use the Picture object to specify the properties of the graphics file to be displayed."
---

# IToPictureInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Picture

The Picture object provides access to a graphic in DIAdem VIEW. You use the Picture object to specify the properties of the graphics file to be displayed.

## Python example

```python
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Picture"
oMyPicture = oMySheet.ActiveArea.DisplayObj
oMyPicture.FileName = dd.ProgramDrv + "Examples/Documents/Course.png"
oMyPicture.KeepRatio = True
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itopictureint-area/">Area</a> | <a href="../../properties/itopictureint-filename/">FileName</a> | <a href="../../properties/itopictureint-keepratio/">KeepRatio</a> | <a href="../../properties/itopictureint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itopictureint-xbegin/">XBegin</a> | <a href="../../properties/itopictureint-xend/">XEnd</a> | <a href="../../properties/itopictureint-ybegin/">YBegin</a> | <a href="../../properties/itopictureint-yend/">YEnd</a> | <a href="../../properties/itopictureint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itopictureint-iszoomed/">IsZoomed</a> | <a href="../../methods/itopictureint-showpicturedlg/">ShowPictureDlg</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Analyzing and Displaying Channels Section by Section</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Background Segments in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Show texts of assignment channels in the VIEW legend</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToPictureInt.htm`*
