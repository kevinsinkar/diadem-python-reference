---
title: "IToTextBoxInt.WordWrap"
description: "Specifies whether DIAdem executes wordwrap automatically in textboxes in DIAdem VIEW."
---

# IToTextBoxInt.WordWrap

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: WordWrap for TextBox

Specifies whether DIAdem executes wordwrap automatically in textboxes in DIAdem VIEW.

## Signature

```python
obj.WordWrap
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj

oMyObj.Text= "Very long text... very long text... " + "very long text... very long text... very long text... very long text... " + "very long text... very long text... very long text... very long text... " + "very long text... very long text... very long text... very long text... " + "Current time: @CurrDate@"

oMyObj.WordWrap = False
oMyObj.ShowScrollBars = "both"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_WordWrap_IToTextBoxInt.htm`*
