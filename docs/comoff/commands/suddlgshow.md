---
title: "SUDDlgShow"
description: "Opens a user dialog box."
---

# SUDDlgShow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SUDDlgShow

Opens a user dialog box.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem first searches the SCRIPT user folder, then the SCRIPT library folder, and finally the DIAdem program folder for a user dialog box to open.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not specify the <span class="Monospace">SudFileName</span> parameter, you must select the dialog box file with the <a href="../suddefload/">SUDDefLoad</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You cannot use the <span class="Monospace">SUDDlgShow</span> command in an <a href="../../../sudref/events/eventinitialize-eventinitialize/">EventInitialize</a> event of a user dialog box.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">SUDDlgShow</span> command displays a modal user dialog box. Use the <a href="../suddlgcreate/">SudDlgCreate</a> command and the method Dialog.<a href="../../../sudref/methods/tosudviewobint-show/">Show</a> to display a non-modal dialog box. Refer to <a href="#" data-unresolved="1">Modal and Non-Modal User Dialog Boxes</a> for further information on working with non-modal dialog boxes.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If data is changed, DIAdem always refreshes the Data Portal in user dialog boxes when the script runs. If you disable refreshing, you speed up the script. To do this, use the <a href="../uiautorefreshset/">UIAutoRefreshSet</a> command. Use the <span class="Monospace">UIAutoRefreshSet</span> command at the end of the script to restore the refresh state to its original value.<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue"><pre><span class="HlVBSKeyword">Dim</span> bRefreshStatus : bRefreshStatus = <span class="HlVBSKeyword">False</span> 
bRefreshStatus = <span class="Hldiademcommand">UiAutoRefreshSet</span>(<span class="HlVBSKeyword">False</span>)
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">SUDDlgShow</span>(<span class="HlString">"Dialog1"</span>,<span class="HlString">"Example.sud"</span>)
<span class="Hldiademcommand">UiAutoRefreshSet</span>(bRefreshStatus)</pre>
</div></td></tr></table>
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
<tr><td width="150">[SUDDlgArgument]</td>
<td>Specifies the transfer parameter for a user dialog box. In the SUD editor you use the methods <a href="../../../sudref/methods/tosudviewob-getargument/">GetArgument</a> and <a href="../../../sudref/methods/tosudviewob-setargument/">SetArgument</a> to access the transfer parameters. The default value of the <span class="Monospace">SUDDlgArgument</span> variable is <span class="Monospace">NULL</span>.<div id="exp_SUDDlgArgument">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the status of a dialog box after you exit the dialog box. The return value is a DlgState type.<div id="exp_DlgState">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"IDOk"</pre></donottranslate></td>
<td>Clicked OK</td></tr>
<tr><td width="150"><donottranslate><pre>"IDCancel"</pre></donottranslate></td>
<td>Clicked Cancel</td></tr>
<tr><td width="150"><donottranslate><pre>"IDNo"</pre></donottranslate></td>
<td>Clicked No</td></tr>
<tr><td width="150"><donottranslate><pre>"IDNoExecute"</pre></donottranslate></td>
<td>Dialog box was not displayed</td></tr>
</table>
</td></tr>
</table>
<p>DIAdem returns the value <span class="Monospace">"IDNoExecute"</span> if the dialog box was not displayed because the value of the variables <a href="../../../varoff/variables/cmdnodialogdisp/">CmdNoDialogDisp</a> or <a href="../../../varoff/variables/cmdnomsgdisp/">CmdNoMsgDisp</a> is <span class="Monospace">TRUE</span>.</p>
</div></td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
bRefreshStatus = UiAutoRefreshSet(False)
SUDDlgShow("Dialog1","Example.sud")
UiAutoRefreshSet(bRefreshStatus)
```

```python
if SUDDlgShow("Dialog1","Example.sud") == "IDOk":
    MsgBoxDisp ("You pressed OK")
```

```python
Class ArgumentHelper
# === Constructor and deconstructor ===
# === MyPara1 property ===
MyPara1  = MyPrivatPara1
End Property
MyPrivatPara1  = ParaNew1
End Property

# === MyPara2 property ===
MyPara2  = MyPrivatPara2
End Property
MyPrivatPara2  = ParaNew2
End Property
End Class

MyArguments = New ArgumentHelper
MyArguments.MyPara1 = "Value 1"
MyArguments.MyPara2 = "Value 2"
if SudDlgShow("MySubDialog",ScriptReadPath + "Example.sud",MyArguments) == "IDOk":
    sgT = "Return values" + "\r\n" + MyArguments.MyPara1 + "\r\n" + MyArguments.MyPara2
    MsgBoxDisp(sgT)
```

```python
def Dialog_EventInitialize(This):
    oDlgParams = This.GetArgument()
    if not (oDlgParams is None) and not isNull(oDlgParams):
        sgT = "Input values" + "\r\n" + oDlgParams.MyPara1 + "\r\n" + oDlgParams.MyPara2
        MsgBoxDisp(sgT)

def OkButton_EventClick(This):
    # write back params
    oDlgParams.MyPara1 = "New Value 1"
    oDlgParams.MyPara2 = "New Value 1"
    Dialog.Ok
```

---

*Source: `ComOff/SUDDlgShow.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
