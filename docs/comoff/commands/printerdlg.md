---
title: "PrinterDlg"
description: "Opens the printer dialog box in DIAdem and changes the print settings without printing the current report."
---

# PrinterDlg

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PrinterDlg

Opens the printer dialog box in DIAdem and changes the print settings without printing the current report.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
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

```python
dd.PrintName = "winspool,\\\\National\\LJ5P,Ne02:"
```

---

*Source: `ComOff/PrinterDlg.htm`*
