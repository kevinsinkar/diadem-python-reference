---
title: "VIEW.Settings"
description: "Specifies the various settings for DIAdem VIEW such as the print margins or the channel reference."
---

# VIEW.Settings

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Settings for View

Specifies the various settings for DIAdem VIEW such as the print margins or the channel reference.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
dd.View.Settings.PrinterRatio = False
dd.View.Settings.PrinterTopMargin = 5
dd.View.Settings.PrinterBottomMargin = 5
dd.View.Settings.PrinterLeftMargin = 5
dd.View.Settings.PrinterRightMargin = 5
dd.View.ActiveSheet.Print()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Settings_VIEW.htm`*
