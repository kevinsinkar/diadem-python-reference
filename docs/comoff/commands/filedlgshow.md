---
title: "FileDlgShow"
description: "Calls the file selection dialog box."
---

# FileDlgShow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FileDlgShow

Calls the file selection dialog box.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileDlgName</td>
<td>Specifies a file. You also can specify the path and the filename extension.<div id="exp_FileDlgName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>You can only use the variable <span class="Monospace">FileDlgName</span> if you assign the value <span class="Monospace">ANY</span> or <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable. If you assign the value <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable, DIAdem interprets the variable <span class="Monospace">FileDlgFilt</span> as the name of the associated DataPlugin.</p>If you do not specify a path in the <span class="Monospace">FileDlgName</span> variable, DIAdem loads the file from the SCRIPT user folder or saves the file in the SCRIPT user folder. If you do not enter a filename extension, DIAdem determines the filename extension from the variable <a href="../../../varoff/variables/filedlgfilt/">FileDlgFilt</a>.<br attr="ext"/>
</div></td></tr>
<tr><td width="150">[FileDlgFilt]</td>
<td>Specifies the file type.<div id="exp_FileDlgFilt">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>The variable <span class="Monospace">FileDlgFilt</span> contains the description and the file filter separated by a comma, for example <span class="Monospace">“Script Files,*.VBS”</span> or <span class="Monospace">“Excel Files, *.csv;*.xls”</span>. You can also specify several file types separated by a vertical line, for example <span class="Monospace">“Script Files,*.VBS|List Files,*.LST”</span>.</p>
<p>In the command <span class="Monospace">FileNameGet</span>, you can only use the variable <span class="Monospace">FileDlgFilt</span> if you assign the value <span class="Monospace">ANY</span> or <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable. If you assign the value <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable, DIAdem interprets the variable <span class="Monospace">FileDlgFilt</span> as the name of the associated DataPlugin.</p>
</div></td></tr>
<tr><td width="150">[FileDlgCaption]</td>
<td>Specifies the dialog box caption.<div id="exp_FileDlgCaption">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>If you do not assign a value to the <span class="Monospace">FileDlgCaption</span> variable, DIAdem generates the caption automatically.</p>
</div></td></tr>
<tr><td width="150">[FileDlgMultiSelect]</td>
<td>Specifies whether one file or multiple files can be selected. The default value is <span class="Monospace">FALSE</span> and specifies that you can select only one file.<div id="exp_FileDlgMultiSelect">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
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

```python
if dd.FileDlgShow(dd.DataReadPath, "TDM Files,*.tdm|DAT Files,*.dat|Excel Files, *.csv;*.xls", "Data selection", False) == "IDOk" :
    dd.DataFileLoad(dd.FileDlgNameList(0))
else:
    print ("The loading of the data was aborted.")
```

```python
dd.FileDlgShow(dd.DataReadPath, "TDM Files,*.tdm|DAT Files,*.dat|Excel Files, *.csv;*.xls", "Data selection", True)
for iCount in range( 0, len(dd.FileDlgNameList)-1):
    dd.DataFileLoad(dd.FileDlgNameList(iCount))
```

---

*Source: `ComOff/FileDlgShow.htm`*
