---
title: "UsedActionObjs"
description: "Collection of all elements used in a bar. The elements that a bar contains are references to elements of the ActionObj collection. When you access a UsedActionO"
---

# UsedActionObjs

!!! abstract "Collection &middot; `ToBarManagerInt.chm`"
    Collection: UsedActionObjs

Collection of all elements used in a bar. The elements that a bar contains are references to elements of the ActionObj collection. When you access a UsedActionObjs collection you receive the element of the ActionObjs collection. To access an individual bar element in a script, use the Item method, or enter the index or the name in parentheses.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If you press &lt;Shift-Ctrl&gt; and idle the cursor on a bar element, DIAdem displays a tooltip with the name of the bar, the name of the bar element, and the name of the base object, which is called the base type. DIAdem also copies this information, separated by a space, to the clipboard.</td>
</tr>
</table>
</div>

## Python example

```python
if dd.BarManager.ActionObjs.Exists("MyButton") :
    oMyActionObj = dd.BarManager.ActionObjs("MyButton")
else:
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton","CustomButton")
    oMyActionObj.Tooltip = "MyButton"
    oMyActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"Hello\")"
    oMyActionObj.Picture = "favicon.ico"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)
```

```python
dd.BarManager.Bars("DIAPanels").UsedActionObjs.Remove("DIAPanelSCRIPT")
```

```python
def CreateActionButton(sID, sIconName, sToolTip, sCommand, oBar):
    if (dd.BarManager.ActionObjs.Exists(sID)) :
        oButtonObj = dd.BarManager.ActionObjs(sID)
    else:
        oButtonObj = dd.BarManager.ActionObjs.Add(sID, "CustomButton")
        oButtonObj.Picture = sIconName
        oButtonObj.Tooltip = sToolTip
        oButtonObj.OnClickCode.Code = sCommand
    oBar.UsedActionObjs.Add(oButtonObj)

def CreateActionPopupObj(sIDName, sIconName, sToolTip, oActionBar, sActionGroup):
# New ActionObject
    if (dd.BarManager.ActionObjs.Exists(sIDName)) :
        oExampleAction = dd.BarManager.ActionObjs(sIDName)
    else:
        oExampleAction = dd.BarManager.ActionObjs.Add(sIDName, "CustomPopup")
        oExampleAction.Picture = sIconName
        oExampleAction.Tooltip = sToolTip
        oExampleAction.BarID = oActionBar.ID

    if not dd.BarManager.Bars(sActionGroup).UsedActionObjs.Exists(oExampleAction) :
        dd.BarManager.Bars(sActionGroup).UsedActionObjs.Add(oExampleAction)

if not dd.BarManager.Bars.Exists("MyBar") :
    oMyBar = dd.BarManager.Bars.Add("MyBar")
else:
    oMyBar = dd.BarManager.Bars("MyBar")
    oMyBar.UsedActionObjs.RemoveAll()

CreateActionButton("MyButton_1", "expl_star_yellow_add.ico", "Starts User Command", "Call MsgBoxDisp(\"User Function\")", oMyBar)
oMyBar.UsedActionObjs.Add("Separator")
CreateActionButton("MyButton_2", "expl_star_yellow_delete.ico", "Deletes Bar", "Call BarManager.Reset", oMyBar)
CreateActionPopupObj("MyPopup", "expl_star_yellow.ico", "Example-Bar", oMyBar, "SCRGroup")
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/tousedactionobjlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tousedactionobjlistint-add/">Add</a> | <a href="../../methods/tousedactionobjlistint-exists/">Exists</a> | <a href="../../methods/tousedactionobjlistint-find/">Find</a> | <a href="../../methods/tousedactionobjlistint-insert/">Insert</a> | <a href="../../methods/tousedactionobjlistint-item/">Item</a> | <a href="../../methods/tousedactionobjlistint-move/">Move</a> | <a href="../../methods/tousedactionobjlistint-remove/">Remove</a> | <a href="../../methods/tousedactionobjlistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/tobarint/">Bar</a>.<a href="../../properties/tobarint-usedactionobjs/">UsedActionObjs</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToUsedActionObjListInt.htm`*
