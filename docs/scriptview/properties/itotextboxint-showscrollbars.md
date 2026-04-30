---
title: "IToTextBoxInt.ShowScrollBars"
description: "Specifies which scroll bars a textbox displays in DIAdem VIEW."
---

# IToTextBoxInt.ShowScrollBars

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: ShowScrollBars for TextBox

Specifies which scroll bars a textbox displays in DIAdem VIEW.

## Signature

```python
obj.ShowScrollBars
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj

oMyObj.Text = "Very long text... Very long text... " + "Very long text... very long text... very long text... very long text... " + "very long text... very long text... very long text... very long text... " + "very long text... very long text... very long text... very long text... " + "Current time: @CurrDate@"

oMyObj.WordWrap = False
oMyObj.ShowScrollBars = "Both"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_ShowScrollBars_IToTextBoxInt.htm`*
