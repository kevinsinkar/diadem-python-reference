---
title: "IToSheetInt.MoveArea"
description: "Moves an area in DIAdem VIEW and splits the specified target area in the same or in another worksheet. Use the Move for Areas method to copy an area within the "
---

# IToSheetInt.MoveArea

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: MoveArea for Sheet

Moves an area in DIAdem VIEW and splits the specified target area in the same or in another worksheet. Use the Move for Areas method to copy an area within the same worksheet. Use the CopyArea for Sheet or the Copy for Areas method to move an area.

## Signature

```python
return_value = obj.MoveArea(SourceAreaNameOrIndex, TargetSheetNameOrIndex, TargetAreaNameOrIndex, enumSplitDirection, Ratio)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSplitTop` | 1 | Top |
| `eSplitBottom` | 2 | Bottom |
| `eSplitLeft` | 3 | Left |
| `eSplitRight` | 4 | Right |

## Python example

```python
oMySheet = dd.View.ActiveSheet
oNewSheet = dd.View.Sheets.Add("MyNewSheet")
oMyMovedArea = oMySheet.MoveArea(1, oMySheet.Index, 1, dd.eSplitRight ,0.25)
```

```python
oMySheet = dd.View.ActiveSheet
oMyMovedArea = oMySheet.MoveArea(1, "", 1, dd.eSplitRight ,0)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a> | <a href="../itosheetint-copyarea/">CopyArea for Sheet</a> | <a href="../itoareaobjectscontint-copy/">Copy for Areas</a> | <a href="../itoareaobjectscontint-move/">Move for Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_MoveArea_IToSheetInt.htm`*
