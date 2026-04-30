---
title: "IToTextBoxInt"
description: "The TextBox object provides access to a Textbox in DIAdem VIEW. You display text and variable contents in the TextBox object."
---

# IToTextBoxInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: TextBox

The TextBox object provides access to a Textbox in DIAdem VIEW. You display text and variable contents in the TextBox object.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.Text= "Current time: @CurrDate@"
oMyFont = oMyObj.Font
oMyFont.Size = 36
oMyFont.Name = "Arial"
oMyFont.Bold = "True"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itotextboxint-alignment/">Alignment</a> | <a href="../../properties/itotextboxint-area/">Area</a> | <a href="../../properties/itotextboxint-bkcolor/">BkColor</a> | <a href="../../properties/itotextboxint-bkcolorrgb/">BkColorRGB</a> | <a href="../../properties/itotextboxint-color/">Color</a> | <a href="../../properties/itotextboxint-colorrgb/">ColorRGB</a> | <a href="../../properties/itotextboxint-font/">Font</a> | <a href="../../properties/itotextboxint-showscrollbars/">ShowScrollBars</a> | <a href="../../properties/itotextboxint-text/">Text</a> | <a href="../../properties/itotextboxint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itotextboxint-wordwrap/">WordWrap</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itotextboxint-refresh/">Refresh</a> | <a href="../../methods/itotextboxint-showtextpropertiesdlg/">ShowTextPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToTextBoxInt.htm`*
