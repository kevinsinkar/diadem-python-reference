---
title: "ToBarInt.Style"
description: "Specifies how the bar elements are displayed within a bar."
---

# ToBarInt.Style

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Style for Bar

Specifies how the bar elements are displayed within a bar.

## Signature

```python
obj.Style
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBarStyleIcon` | 0 | DIAdem displays only the graphic. |
| `eBarStyleCaption` | 1 | DIAdem displays only the text. |
| `eBarStyleIconCaption` | 2 | DIAdem displays the text on the right side of the graphic. |
| `eBarStyleIconCaptionBelow` | 3 | DIAdem displays the text below the graphic. |

## Python example

```python
dd.Barmanager.Bars("SCRMain").Style = dd.eBarStyleIconCaptionBelow
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Style_ToBarInt.htm`*
