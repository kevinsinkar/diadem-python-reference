---
title: "AutEdOpenDlg"
description: "Opens the load dialog box in the script editor and loads the file that you select in this dialog box."
---

# AutEdOpenDlg

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AutEdOpenDlg

Opens the load dialog box in the script editor and loads the file that you select in this dialog box.

## Signature

```python
dd.AutEdOpenDlg([AutEdSyntax])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[AutEdSyntax]</td>
<td>Specifies the syntax of the loaded file.<div id="exp_AutEdSyntax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p>Possible values are:</p>
<table class="Borderless"><tr><td width="150">VBS DIADEM</td><td>Uses the syntax support for DIAdem VBS scripts in the script editor.</td></tr><tr><td width="150">VBS-DATA-PLUGIN</td><td>Uses the syntax support for DataPlugin scripts in the script editor.</td></tr></table>
<p>If you do not specify a value, DIAdem uses the value <span class="Monospace">VBS DIADEM</span>.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/AutEdOpenDlg.htm`*
