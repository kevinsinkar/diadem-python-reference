---
title: "ToBarInt.Position"
description: "Specifies where the bar is positioned in the higher-ranking window."
---

# ToBarInt.Position

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Position for Bar

Specifies where the bar is positioned in the higher-ranking window.

## Signature

```python
obj.Position
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBarPositionAuto` | 0 | DIAdem specifies the position automatically (default). |
| `eBarPositionTop` | 1 | Positioned at the top of the window. |
| `eBarPositionLeft` | 2 | Positioned at the left edge of the window. |

## Python example

```python
dd.MsgBoxDisp("Position : " + dd.BarManager.Bars("SCRMain").Position)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Position_ToBarInt.htm`*
