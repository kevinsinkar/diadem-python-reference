---
title: "ToPropPictureInt"
description: "The Picture object specifies the graphics file (*.ico) with which a bar element appears on the DIAdem interface. For DIAdem to display a graphic, the graphics f"
---

# ToPropPictureInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: Picture

The Picture object specifies the graphics file (*.ico) with which a bar element appears on the DIAdem interface. For DIAdem to display a graphic, the graphics file must contain a symbol that is same size as the properties ActionObjPictureHeight and ActionObjPictureWidth of the bar that is to contain the symbol. DIAdem uses 16*16 pixels as the default size for symbols on the toolbars and on the menu bars, and either 32*32 pixel, 48*48 pixel, or 64*64 pixel for symbols on the group bars. User-defined graphic files should all contain these sizes. The graphics file must be in the Resource folder . The specifications ActionObjPictureWidth and ActionObjPictureHeight refer to a screen resolution of 96 DPI. With other screen resolutions, DIAdem either scales the graphic or uses a matching symbol size from the ICO file. For example, if the resolution is 44 DPI, DIAdem scales the graphic by 150% or uses a 24 pixel-sized symbol, if that is available in the ICO file, for 16 pixel-sized specifications. If DIAdem cannot display a symbol, the bar element is displayed with one of the following symbols: DIAdem displays this symbol if the graphics file is not in the resource folder and the bar is not displayed as a menu so that Style for Bar does not contain the values eBarStyleIcon or eBarStyleIconCaptionBelow . If you want to display the bar as a menu with a graphic, which means that Style = eBarStyleIconCaption and the graphic are not found, DIAdem does not display a symbol. DIAdem displays this symbol if the bar contains a reference to an element that does not exist in the ActionObjs collection.

## Notes

<div markdown="1">
<table class="Borderless" id="table3">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>To create your own ICO files you require an appropriate graphics program, for example you could buy Axialis IconWorkshop (www.axialis.com) (www.axialis.com) or use the program IcoFX (www.icofx.ro). In DIAdem you also can use the <a href="../../../comoff/commands/imagefiletoiconfile/">ImageFileToIconFile</a> command to convert a graphic file into an ICO file.</td>
</tr>
</table>
</div>

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyObjButton1")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyObjButton1", "CustomButton")
    oMyActionObj.Picture = "favicon.ico"
    oMyActionObj.Tooltip = "MyObjButton1"
    oMyActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"MyObjButton1\")"
dd.BarManager.Bars("ANAMain").UsedActionObjs.Add(oMyActionObj)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/toproppictureint-filename/">FileName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../toactionobjbuttonint/">ActionObjButton</a>.<a href="../../properties/toactionobjbuttonint-picture/">Picture</a> | <a href="../toactionobjcheckint/">ActionObjCheckbutton</a>.<a href="../../properties/toactionobjcheckint-picture/">Picture</a> | <a href="../toactionobjpopupint/">ActionObjPopup</a>.<a href="../../properties/toactionobjpopupint-picture/">Picture</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToPropPictureInt.htm`*
