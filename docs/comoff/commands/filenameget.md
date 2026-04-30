---
title: "FileNameGet"
description: "Opens the standard dialog box for loading and saving files."
---

# FileNameGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FileNameGet

Opens the standard dialog box for loading and saving files.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileTargetDevice</td>
<td>Specifies the DIAdem panel for which you load or save a file.<div id="exp_FileTargetDevice">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NAVIGATOR"</pre></donottranslate></td>
<td>DIAdem NAVIGATOR panel</td></tr>
<tr><td width="150"><donottranslate><pre>"REPORT"</pre></donottranslate></td>
<td>DIAdem REPORT panel</td></tr>
<tr><td width="150"><donottranslate><pre>"DAC"</pre></donottranslate></td>
<td>DIAdem DAC panel</td></tr>
<tr><td width="150"><donottranslate><pre>"ANY"</pre></donottranslate></td>
<td>Any DIAdem panel</td></tr>
<tr><td width="150"><donottranslate><pre>"VIEW"</pre></donottranslate></td>
<td>DIAdem VIEW panel</td></tr>
<tr><td width="150"><donottranslate><pre>"SCRIPT"</pre></donottranslate></td>
<td>SCRIPT</td></tr>
</table>
</td></tr>
</table>
<p>You can only use the variable <span class="Monospace">FileDlgFilt</span> if you assign the value <span class="Monospace">ANY</span> or <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable. If you assign the value <span class="Monospace">NAVIGATOR</span> to the <span class="Monospace">FileTargetDevice</span> variable, DIAdem interprets the variable <span class="Monospace">FileDlgFilt</span> as the name of the associated DataPlugin.</p>
</div></td></tr>
<tr><td width="150">FileOperation</td>
<td>Specifies whether you load a file or save a file.<div id="exp_FileOperation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"FileRead"</pre></donottranslate></td>
<td>File selection for reading</td></tr>
<tr><td width="150"><donottranslate><pre>"FileWrite"</pre></donottranslate></td>
<td>File selection for writing</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[FileDlgName]</td>
<td>Specifies a file. You can also specify the path and the filename extension.<div id="exp_FileDlgName">
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
<tr><td width="150">[FileDlgASCIIName]</td>
<td>Specifies the ASCII file where you save the names of the files that you selected in the dialog box for opening and saving files.<div id="exp_FileDlgASCIIName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 255 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="body">You only can select several files simultaneously for loading and saving if you assign a filename to the <span class="Monospace">FileDlgASCIIName</span> variable.</p>
<p>You can use the variables <span class="Monospace">FileDlgASCIIName</span> and <span class="Monospace">FileDlgPathKey</span> if you assign the value <span class="Monospace">ANY</span> to the <span class="Monospace">FileTargetDevice</span> variable.</p>
<p>The variable <a href="../../../varoff/variables/filedlgpathkey/">FileDlgPathKey</a> specifies whether DIAdem stores the filenames with absolute paths.</p>
<p>You can assign a filename with a path and a filename extension to the <span class="Monospace">FileDlgASCIIName</span> variable. If you do not specify a path, DIAdem saves the file in the current SCRIPT user folder. If you do not specify a filename extension, DIAdem uses the extension <span class="Monospace">Lst</span>.<br attr="ext"/>If the file specified in the variable <span class="Monospace">FileDlgASCIIName</span> already exists, DIAdem overwrites this file.</p>
</div></td></tr>
<tr><td width="150">[FileDlgPathKey]</td>
<td>Specifies whether DIAdem stores the names of the selected files with absolute paths or without paths in the ASCII file. The default value is <span class="Monospace">FALSE</span> which specifies that DIAdem does not save the absolute path as well.<div id="exp_FileDlgPathKey">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>You can use the variables <span class="Monospace">FileDlgASCIIName</span> and <span class="Monospace">FileDlgPathKey</span> if you assign the value <span class="Monospace">ANY</span> to the <span class="Monospace">FileTargetDevice</span> variable. Specify the ASCII file with the <a href="../../../varoff/variables/filedlgasciiname/">FileDlgASCIIName</a> variable.</p>
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
dd.FileNameGet("ANY", "FileRead", dd.DataReadPath, "TDM data (*.tdm),*.tdm", "All.lst", True, "Data selection")
MyFileNames = dd.FileDlgFileName.split("|")
for iCount in range(len(MyFileNames)):
    dd.DataFileLoad(MyFileNames[iCount])
```

```python
if (dd.FileNameGet( "REPORT", "FileRead", dd.LayoutReadPath + ".TDR") == "IDOk") : # Dialog closed with Ok
    dd.Report.LoadLayout(dd.FileDlgFileName)
    dd.Report.Refresh()
```

```python
if (dd.FileNameGet("NAVIGATOR", "FileRead", dd.DataReadPath + ".TDM") == "IDOk") : # Dialog closed with Ok
    if dd.FileDlgPartial :
# Open dialog to select channels, then load or register
        dd.DataFileSelDlg(dd.FileDlgFileName,dd.FileDlgFilter)
    else:
# Load or register all channels
        dd.DataFileLoad(dd.FileDlgFileName,dd.FileDlgFilter,dd.FileDlgImpAction)
```

```python
if (dd.FileNameGet("REPORT", "FileWrite", dd.LayoutReadPath +  "*.TDR") == "IDOk") : # Dialog closed with Ok
    dd.Report.SaveLayout(dd.FileDlgFileName)
```

```python
if (dd.FileNameGet ("NAVIGATOR", "FileWrite", dd.DataReadPath + dd.Data.Root.Properties("name").Value + "." + dd.DataExtension) == "IDOk") :
    if dd.FilEx(dd.FileDlgFileName) : #File exists
        dd.MsgBoxDisp("File " + dd.FileDlgFileName + " exists. Overwrite?","MB_YESNO")
        if (dd.MsgState == "IDYes") :
            if (dd.FileDlgPartial== True) : #Use selected channels
                dd.DataFileSaveSel(dd.FileDlgFileName, dd.FileDlgFilter, dd.Portal.ActiveView.Selection)
            else:
                dd.DataFileSave(dd.FileDlgFileName, dd.FileDlgFilter )
        else: #Dialog was canceled
            dd.MsgBoxDisp ("Data saving was canceled")
    else: #File does not exist
        if (dd.FileDlgPartial== True) : #Use selected channels
            dd.DataFileSaveSel(dd.FileDlgFileName, dd.FileDlgFilter, dd.Portal.ActiveView.Selection)
        else:
            dd.DataFileSave(dd.FileDlgFileName, dd.FileDlgFilter )
else: #Dialog was canceled
    dd.MsgBoxDisp ("Data saving was canceled")
```

---

*Source: `ComOff/FileNameGet.htm`*
