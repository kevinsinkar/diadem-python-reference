---
title: "ToBarManagerUIInt"
description: "Use the BarManager object to access the panels, bar, and bar elements of DIAdem. Use the BarManager object to load and to save the bar definitions. The BarManag"
---

# ToBarManagerUIInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: BarManager

Use the BarManager object to access the panels, bar, and bar elements of DIAdem. Use the BarManager object to load and to save the bar definitions. The BarManager object is available as a global object in scripts and in dialog boxes, and represents the visible bars.

## Python example

```python
for panel in dd.BarManager.Panels:
  bar_ids = []
  for bar in panel.UsedBars:
    bar_ids.append(bar.ID)
  print(f"{panel.ID:10}", "Bars:", bar_ids)
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
<p><a href="../../properties/tobarmanageruiint-actionobjs/">ActionObjs</a> | <a href="../../properties/tobarmanageruiint-bars/">Bars</a> | <a href="../../properties/tobarmanageruiint-dataportal/">DataPortal</a> | <a href="../../properties/tobarmanageruiint-desktopmodified/">DesktopModified</a> | <a href="../../properties/tobarmanageruiint-filename/">FileName</a> | <a href="../../properties/tobarmanageruiint-filepath/">FilePath</a> | <a href="../../properties/tobarmanageruiint-panels/">Panels</a> | <a href="../../properties/tobarmanageruiint-resourcepath/">ResourcePath</a> | <a href="../../properties/tobarmanageruiint-shell/">Shell</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tobarmanageruiint-addmenubar/">AddMenuBar</a> | <a href="../../methods/tobarmanageruiint-addmenuitem/">AddMenuItem</a> | <a href="../../methods/tobarmanageruiint-create/">Create</a> | <a href="../../methods/tobarmanageruiint-createfromdeployment/">CreateFromDeployment</a> | <a href="../../methods/tobarmanageruiint-import/">Import</a> | <a href="../../methods/tobarmanageruiint-ismodified/">IsModified</a> | <a href="../../methods/tobarmanageruiint-load/">Load</a> | <a href="../../methods/tobarmanageruiint-refresh/">Refresh</a> | <a href="../../methods/tobarmanageruiint-reset/">Reset</a> | <a href="../../methods/tobarmanageruiint-save/">Save</a> | <a href="../../methods/tobarmanageruiint-saveasdeployment/">SaveAsDeployment</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="./">BarManager</a>.<a href="../../methods/tobarmanageruiint-create/">Create</a> | <a href="./">BarManager</a>.<a href="../../methods/tobarmanageruiint-createfromdeployment/">CreateFromDeployment</a> | <a href="../tobarmanagerint/">BarManagerUnattached</a>.<a href="../../methods/tobarmanagerint-create/">Create</a> | <a href="../tobarmanagerint/">BarManagerUnattached</a>.<a href="../../methods/tobarmanagerint-createfromdeployment/">CreateFromDeployment</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToBarManagerUIInt.htm`*
