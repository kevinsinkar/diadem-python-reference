---
title: "MsgBoxDisp"
description: "Displays a message in a message box."
---

# MsgBoxDisp

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MsgBoxDisp

Displays a message in a message box.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you use the <a href="./">MsgBoxDisp</a> command to open a message box and if the <a href="../../../varoff/variables/msgtype/">MsgType</a> variable has the value <span class="Monospace">MsgTypeWarning</span>, DIAdem ignores the value of the <span class="Monospace">MsgNotModal</span> variable and always opens the message box modally.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem evaluates the <span class="Monospace">MsgButtonType</span> variable only if the <span class="Monospace">MsgType</span> variable has the value <span class="Monospace">MsgTypeNote</span> or the value <span class="Monospace">MsgTypeWarning</span>.  A message without keys is only possible for non-modal message boxes. The <span class="Monospace">MsgType</span> variable must have the value <span class="Monospace">MsgTypeNote</span>, the <span class="Monospace">MsgButtonType</span> variable must have the value <span class="Monospace">MB_NOBUTTON,</span> and the <span class="Monospace">MsgNotModal</span> variable must have the value <span class="Monospace">TRUE</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the <span class="Monospace">Msgtype</span> variable has the value <span class="Monospace">MsgTypeError</span>, the script aborts when the message displays. If the <span class="Monospace">Msgtype</span> variable has other values, DIAdem continues the script after displaying a message.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">MsgText</td>
<td>Specifies the text of a message.<div id="exp_MsgText">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[MsgButtonType]</td>
<td>Specifies the type and number of buttons in a message box. The default value of the <span class="Monospace">MsgButtonType</span> variable is <span class="Monospace">MB_OK</span>.<div id="exp_MsgButtonType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"MB_OK"</pre></donottranslate></td>
<td>OK button</td></tr>
<tr><td width="150"><donottranslate><pre>"MB_OKCANCEL"</pre></donottranslate></td>
<td>OK/Cancel button</td></tr>
<tr><td width="150"><donottranslate><pre>"MB_RETRYCANCEL"</pre></donottranslate></td>
<td>Repeat/Cancel button</td></tr>
<tr><td width="150"><donottranslate><pre>"MB_YESNO"</pre></donottranslate></td>
<td>Yes/No button</td></tr>
<tr><td width="150"><donottranslate><pre>"MB_YESNOCANCEL"</pre></donottranslate></td>
<td>Yes/No/Cancel button</td></tr>
<tr><td width="150"><donottranslate><pre>"MB_ABORTRETRYIGNORE"</pre></donottranslate></td>
<td>Exit/Repeat/Ignore button</td></tr>
<tr><td width="150"><donottranslate><pre>"MB_NOBUTTON"</pre></donottranslate></td>
<td>No button</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[MsgType]</td>
<td>Specifies the type of a message box. The default value of the <span class="Monospace">MsgType</span> variable is <span class="Monospace">MsgTypeNote</span>.<div id="exp_MsgType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"MsgTypeNote"</pre></donottranslate></td>
<td>Message box</td></tr>
<tr><td width="150"><donottranslate><pre>"MsgTypeError"</pre></donottranslate></td>
<td>Error box</td></tr>
<tr><td width="150"><donottranslate><pre>"MsgTypeWarning"</pre></donottranslate></td>
<td>Warning box</td></tr>
<tr><td width="150"><donottranslate><pre>"MsgTypeInformation"</pre></donottranslate></td>
<td>Information box</td></tr>
<tr><td width="150"><donottranslate><pre>"MsgTypeAlert"</pre></donottranslate></td>
<td>Script continue error box</td></tr>
<tr><td width="150"><donottranslate><pre>"MsgTypeNoteNoIcon"</pre></donottranslate></td>
<td>Message box without icon</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[MsgStdButton]</td>
<td>Specifies the standard button for a message box. The default value of the <span class="Monospace">MsgStdButton</span> variable is <span class="Monospace">0</span>.<div id="exp_MsgStdButton">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
<td>0 &lt;= MsgStdButton &lt;= 3</td></tr>
</table>
<p class="Body"><strong>Valid settings</strong></p>
<table class="Borderless"><tr><td width="150">0 or 1</td><td>First button (default setting)</td></tr><tr><td width="150">2</td><td>Second button</td></tr><tr><td width="150">3</td><td>Third button</td></tr></table>
<p class="Body">If a message box has fewer buttons than the <span class="Monospace">MsgStdButton</span> specifies, DIAdem uses the default value.</p>
</div></td></tr>
<tr><td width="150">[MsgTimeOut]</td>
<td>Specifies how many seconds elapse before DIAdem closes a message box. The default value of the <span class="Monospace">MsgTimeOut</span> variable is <span class="Monospace">0</span>.<div id="exp_MsgTimeOut">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= MsgTimeOut &lt;= 1000000</td></tr>
</table>
<p class="Body">If the <span class="Monospace">MsgTimeOut</span> variable contains the value <span class="Monospace">0</span>, the message box closes independently.</p>
</div></td></tr>
<tr><td width="150">[MsgNotModal]</td>
<td>Specifies whether DIAdem opens a message box modally or non-modally. The default value is <span class="Monospace">FALSE</span> which means that DIAdem opens the message box in modal mode.<div id="exp_MsgNotModal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If you assign the value <span class="Monospace">FALSE</span> to the <span class="Monospace">MsgNotModal</span> variable, the message box is modal. DIAdem does not continue a script until the user closes the message box. If you assign the value <span class="Monospace">TRUE</span> to the <span class="Monospace">MsgNotModal</span> variable, the message box is modal. DIAdem continues a script immediately.</p>
<p class="Body">If DIAdem displays another non-modal message box during the script, the new message box replaces the previous message box.</p>
<p class="Body">Use the <a href="../msgboxcancel/">MsgBoxCancel</a> command to close a message box. Alternatively, use the <a href="../../../varoff/variables/msgtimeout/">MsgTimeOut</a> variable to specify how long DIAdem waits before it closes the message box automatically.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you use the <a href="./">MsgBoxDisp</a> command to open a message box and if the <a href="../../../varoff/variables/msgtype/">MsgType</a> variable has the value <span class="Monospace">MsgTypeWarning</span>, DIAdem ignores the value of the <span class="Monospace">MsgNotModal</span> variable and always opens the message box modally.</td></tr></table>
</div></td></tr>
<tr><td width="150">[MsgNo]</td>
<td>For future extensions.</td></tr>
<tr><td width="150">[MsgSrc]</td>
<td>For future extensions.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the type of button you used to exit a message box. The return value is a MsgState type.<div id="exp_MsgState">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"IDAbort"</pre></donottranslate></td>
<td>Clicked Close</td></tr>
<tr><td width="150"><donottranslate><pre>"IDCancel"</pre></donottranslate></td>
<td>Clicked Cancel</td></tr>
<tr><td width="150"><donottranslate><pre>"IDIgnore"</pre></donottranslate></td>
<td>Clicked Ignore</td></tr>
<tr><td width="150"><donottranslate><pre>"IDNo"</pre></donottranslate></td>
<td>Clicked No</td></tr>
<tr><td width="150"><donottranslate><pre>"IDOk"</pre></donottranslate></td>
<td>Clicked OK</td></tr>
<tr><td width="150"><donottranslate><pre>"IDRetry"</pre></donottranslate></td>
<td>Clicked Retry</td></tr>
<tr><td width="150"><donottranslate><pre>"IDYes"</pre></donottranslate></td>
<td>Clicked Yes</td></tr>
<tr><td width="150"><donottranslate><pre>"IDNone"</pre></donottranslate></td>
<td>Clicked None</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.MsgBoxSetPos(10, 10, 30, 20)
dd.MsgButtonTextSet("Step+1", "Step+2", "Step+3")
select_variable_0 = dd.MsgBoxDisp("Select next step","MB_YESNOCANCEL")
if (select_variable_0 == "IDYes") :
    dd.MsgBoxDisp("Step 1", "MB_OK", "MsgTypeNote",None , 5)
elif (select_variable_0 == "IDNo") :
    dd.MsgBoxDisp("Step 2", "MB_OK", "MsgTypeInformation",None , 5)
elif (select_variable_0 == "IDCancel") :
    dd.MsgBoxDisp("Step 3", "MB_OK", "MsgTypeWarning",None , 5)
dd.MsgNotModal = True
dd.MsgBoxDisp("Example completed", "MB_NOBUTTON", "MsgTypeNote",None , 10, True)
```

---

*Source: `ComOff/MsgBoxDisp.htm`*
