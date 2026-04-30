---
title: "ITo3DCurveInt.Name"
description: "Specifies the name of an order line in a cascade display in DIAdem VIEW. A curve is identified by its name, which means that the curve name must be unique and m"
---

# ITo3DCurveInt.Name

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Name for Line

Specifies the name of an order line in a cascade display in DIAdem VIEW. A curve is identified by its name, which means that the curve name must be unique and may not be used more than once.

## Signature

```python
obj.Name
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\cascade.tdm","TDM","")
dd.View.NewLayout()
dd.View.Sheets(1).Areas(1).DisplayObjType = "Cascade"
oMyDisplayObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyCascadeCurve = oMyDisplayObj.CurvesCascade.AddCascade("[2]/[1]","[2]/[2]","[2]/[3]")
oMyLineCurve = oMyDisplayObj.CurvesCascade.AddLine("[4]/[156]","[4]/[157]")
dd.MsgBoxDisp("Name of new curve: " + oMyLineCurve.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Name_ITo3DCurveInt.htm`*
