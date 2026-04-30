---
title: "ActionObjs"
description: "Collection of all bar elements in DIAdem. To access an individual bar element in a script, use the Item property, or enter the index or the name in parentheses."
---

# ActionObjs

!!! abstract "Collection &middot; `ToBarManagerInt.chm`"
    Collection: ActionObjs

Collection of all bar elements in DIAdem. To access an individual bar element in a script, use the Item property, or enter the index or the name in parentheses.

## Python example

```python
if dd.BarManager.ActionObjs.Exists("MyButton") :
    oMyActionObj = dd.BarManager.ActionObjs("MyButton")
else:
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton","CustomButton")
    oMyActionObj.Tooltip = "MyButton"
    oMyActionObj.Picture = "favicon.ico"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)
```

```python
if dd.BarManager.ActionObjs.Exists("MyPopup") :
    dd.BarManager.ActionObjs.Remove("MyPopup")
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
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/toactionobjlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/toactionobjlistint-add/">Add</a> | <a href="../../methods/toactionobjlistint-copy/">Copy</a> | <a href="../../methods/toactionobjlistint-exists/">Exists</a> | <a href="../../methods/toactionobjlistint-getuniqueid/">GetUniqueID</a> | <a href="../../methods/toactionobjlistint-item/">Item</a> | <a href="../../methods/toactionobjlistint-remove/">Remove</a> | <a href="../../methods/toactionobjlistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/tobarmanageruiint/">BarManager</a>.<a href="../../properties/tobarmanageruiint-actionobjs/">ActionObjs</a> | <a href="../../objects/tobarmanagerint/">BarManagerUnattached</a>.<a href="../../properties/tobarmanagerint-actionobjs/">ActionObjs</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToActionObjListInt.htm`*
