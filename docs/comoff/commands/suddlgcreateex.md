---
title: "SUDDlgCreateEx"
description: "Generates a non-modal SUD dialog box."
---

# SUDDlgCreateEx

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SUDDlgCreateEx

Generates a non-modal SUD dialog box.

## Signature

```python
return_value = dd.SUDDlgCreateEx(SUDDlgName, SUDFileName, SUDDlgAliasName , SUDDlgkeepEnabled )
```

## Notes

<div markdown="1">
<table class="Borderless" id="table8"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>Only set the <span class="Monospace">SUDDlgkeepEnabled</span> variable to <span class="Monospace">True</span>, if other dialog boxes or scripts do not impact the objects used in the dialog box. Otherwise unexpected errors might occur.</td></tr></table>
<table class="Borderless" id="table5"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>Use the methods Dialog.<a href="../../../sudref/methods/tosudviewobint-show/">Show</a> and Dialog.<a href="../../../sudref/methods/tosudviewobint-hide/">Hide</a> to display and to hide a non-modal user dialog box. Use the methods Dialog.<a href="../../../sudref/methods/tosudviewobint-ok/">OK</a> and Dialog.<a href="../../../sudref/methods/tosudviewobint-cancel/">Cancel</a> to close the non-modal dialog box. Refer to <a href="#" data-unresolved="1">Modal and Non-Modal User Dialog Boxes</a> for further information on working with non-modal dialog boxes.</td></tr></table>
<table class="Borderless" id="table7"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>Use the Dialog.<a href="../../../sudref/properties/tosudviewobint-filename/">Filename</a> variable instead of the <a href="../../../varoff/variables/autoactpath/">AutoActPath</a> variable in a non-modal user dialog box.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If data is changed, DIAdem always refreshes the Data Portal in user dialog boxes when the script runs. If you disable refreshing, you speed up the script. To do this, use the <a href="../uiautorefreshset/">UIAutoRefreshSet</a> command. Use the <span class="Monospace">UIAutoRefreshSet</span> command at the end of the script to restore the refresh state to its original value.<br attr="ext"/>If you disabled the refresh mode in a non-modal dialog box with the <span class="Monospace">UIAutoRefreshSet</span> command, you must enable the refresh mode with the <span class="Monospace">UIAutoRefreshSet</span> command when the <a href="../../../sudref/events/eventterminate-eventterminate/">EventTerminate</a> event occurs at the latest. If you used the <a href="../scriptstart/">ScriptStart</a> command to call a script from the non-modal dialog box, DIAdem refreshes the data changes automatically when the script is finished. </td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SUDDlgName</td>
<td>Specifies the name of a user dialog box to be displayed.<div id="exp_SUDDlgName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SUDFileName</td>
<td>Specifies the name of a SUD file. By default the <span class="Monospace">SUDFileName</span> variable contains an empty text.<div id="exp_SUDFileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SUDDlgAliasName</td>
<td>Specifies the alias name for a user dialog box.<div id="exp_SUDDlgAliasName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">SUDDlgkeepEnabled</td>
<td>Specifies whether the user dialog box is disabled when other dialog boxes are open or scripts are running.<div id="exp_SUDDlgkeepEnabled">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="../../../sudref/objects/tosudviewobint/">Dialog<nonmodal>Object</nonmodal></a> type.</td></tr>
</table>
</div>

## Python example

```python
MyFileName = dd.ScriptReadPath + "MyTestDialog.SUD"
if None is dd.SudNonModalDlgLst("MyDialog1") :
    MyDlg1 = dd.SUDDlgCreateEx("Dlg1",MyFileName,"MyDialog1",True)
    MyDlg1.Color = dd.RGB(255, 0, 0)
else:
    MyDlg1.Cancel
if None is dd.SudNonModalDlgLst("MyDialog2") :
    MyDlg2 = dd.SUDDlgCreateEx("Dlg1",MyFileName,"MyDialog2",True)
    MyDlg2.Color = dd.RGB(0, 0, 255)
else:
    MyDlg2.Cancel
MyDlg1.Show
MyDlg1.Move (20,20)
MyDlg2.Show
```

---

*Source: `ComOff/SUDDlgCreateEx.htm`*
