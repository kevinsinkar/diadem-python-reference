---
title: "ToBarManagerUIInt.Refresh"
description: "Rebuilds the bars of the DIAdem main window and all visible, used bars of the current panel and refreshes the display. DIAdem automatically refreshes the displa"
---

# ToBarManagerUIInt.Refresh

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Refresh for BarManager

Rebuilds the bars of the DIAdem main window and all visible, used bars of the current panel and refreshes the display. DIAdem automatically refreshes the display when scripts start or end, when the user switches panels, and when the user clicks a bar element. Therefore you do not need to call the Refresh method in a script. Use the Refresh method in the VBS code of modal and non-modal dialog boxes.

## Signature

```python
obj.Refresh
```

## Python example

```python
def Button1_EventClick():
    if dd.BarManager.ActionObjs.Exists("MyButton") :
        oMyActionObj = dd.BarManager.ActionObjs("MyButton")
    else:
        oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton","CustomButton")
        oMyActionObj.Tooltip = "MyButton"
        oMyActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"Hello\")"
        oMyActionObj.Picture = "favicon.ico"
    dd.BarManager.Shell.UsedBars(1).UsedActionObjs.Add(oMyActionObj)
    dd.Barmanager.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Refresh_ToBarManagerUIInt.htm`*
