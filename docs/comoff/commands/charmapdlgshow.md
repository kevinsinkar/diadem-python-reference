---
title: "CharMapDlgShow"
description: "Opens the dialog box of the character table."
---

# CharMapDlgShow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CharMapDlgShow

Opens the dialog box of the character table.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CharMapText</td>
<td>Receives the character selected in the character table.<div id="exp_CharMapText">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">CharMapFont</td>
<td>Specifies the name of the font in the dialog box of the character table.<div id="exp_CharMapFont">
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

---

*Source: `ComOff/CharMapDlgShow.htm`*
