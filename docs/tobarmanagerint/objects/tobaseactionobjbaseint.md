---
title: "ToBaseActionObjBaseInt"
description: "The ActionObj provides an element in a bar, which appears as a symbol on the interface. You can use an ActionObj object in one or more bars. An ActionObj object"
---

# ToBaseActionObjBaseInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: ActionObj

The ActionObj provides an element in a bar, which appears as a symbol on the interface. You can use an ActionObj object in one or more bars. An ActionObj object has a base object or base type that defines which task the ActionObj object executes. For example, the ANADlgChnAdd base type specifies that DIAdem opens a dialog box for the summation of channels. Under certain conditions you can change an ActionObj object that has a base type which refers to a specific function. The function of the ActionObj object remains the same. If you want to create an ActionObj object with any functionality, you can use the base types CustomButton , CustomCheckButton , and CustomPopup . The ActionObj corresponds to one of the following objects: ActionObjButton (ToActionObjButtonInt) Button ActionObjCheckbutton (ToActionObjCheckInt) Button that displays a status. ActionObjPopup (ToActionObjPopupInt) Button that opens a sub-bar. ActionObjSeparator (ToActionObjSeparatorInt) Separator

## Python example

```python
dd.BarManager.ActionObjs.Copy("ANADlgChnAdd","MyANADlgChnAdd")
dd.BarManager.ActionObjs("MyANADlgChnAdd").Tooltip = "My channel add function"
dd.Barmanager.Bars("ANAMain").UsedActionObjs.Insert("MyANADlgChnAdd",5)
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
<p><a href="../../properties/tobaseactionobjbaseint-id/">ID</a> | <a href="../../properties/tobaseactionobjbaseint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-add/">Add</a> | <a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-copy/">Copy</a> | <a href="../../collections/actionobjs/">ActionObjs</a>.<a href="../../methods/toactionobjlistint-item/">Item</a> | <a href="../../collections/usedactionobjs/">UsedActionObjs</a>.<a href="../../methods/tousedactionobjlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToBaseActionObjBaseInt.htm`*
