---
title: "SUDDlgCreate"
description: "Generates a non-modal SUD dialog box."
---

# SUDDlgCreate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SUDDlgCreate

Generates a non-modal SUD dialog box.

## Signature

```python
return_value = dd.SUDDlgCreate(SUDDlgName, SUDFileName)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table5"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>Use the methods Dialog.<a href="../../../sudref/methods/tosudviewobint-show/">Show</a> and Dialog.<a href="../../../sudref/methods/tosudviewobint-hide/">Hide</a> to display and to hide a non-modal user dialog box. Use the methods Dialog.<a href="../../../sudref/methods/tosudviewobint-ok/">OK</a> and Dialog.<a href="../../../sudref/methods/tosudviewobint-cancel/">Cancel</a> to close the non-modal dialog box. Refer to <a href="#" data-unresolved="1">Modal and Non-Modal User Dialog Boxes</a> for further information on working with non-modal dialog boxes.</td></tr></table>
<table class="Borderless" id="table6"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>The <span class="Monospace">SudDlgCreate</span> command can open a specified user dialog box only once in non-modal mode. Use the <a href="../sudnonmodaldlglst/">SudNonModalDlgLst</a> command to receive a list of non-modal user dialog boxes that are already open. If you want to open several dialog boxes at the same time, use the <a href="../suddlgcreateex/">SUDDlgCreateEx</a> command.</td></tr></table>
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
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="../../../sudref/objects/tosudviewobint/">Dialog object</a> type. To create a Dialog object, you assign the returned object to an object variable.</td></tr>
</table>
</div>

## Python example

```python
if None is dd.SudNonModalDlgLst("Dialog1") :
    MyDlg = dd.SudDlgCreate("Dialog1","Example")
else:
    MyDlg = dd.SudNonModalDlgLst("Dialog1")

MyDlg.Show()
```

---

*Source: `ComOff/SUDDlgCreate.htm`*
