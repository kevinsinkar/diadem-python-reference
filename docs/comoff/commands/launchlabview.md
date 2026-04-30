---
title: "LaunchLabVIEW"
description: "Starts the LabVIEW program and opens a VI."
---

# LaunchLabVIEW

!!! abstract "Command &middot; `ComOff.chm`"
    Command: LaunchLabVIEW

Starts the LabVIEW program and opens a VI.

## Signature

```python
dd.LaunchLabVIEW([LVTemplateVI])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you click the LabVIEW button in the DIAdem panel bar, DIAdem executes the <span class="Monospace">LaunchLabVIEW</span> command.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[LVTemplateVI]</td>
<td>Specifies the VI that LabVIEW opens when you start LabVIEW from DIAdem.<div id="exp_LVTemplateVI">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">Use the <a href="../../../varoff/variables/lvtemplatepath/">LVTemplatePath</a> variable to specify the path that the VI is on. Use the <a href="./">LaunchLabVIEW</a> command to start LabVIEW.</p>
<p class="Body">If you do not specify the VI, LabVIEW opens the introduction screen.</p>
</div></td></tr>
</table>
</div>

## Python example

```python
if dd.IsAvailLabVIEW :
    dd.LVTemplateVI = "About.vit"
    dd.LVTemplatePath = "Templates\\"
    dd.LaunchLabVIEW()
else:
    dd.MsgBoxDisp("LabVIEW is not installed.")
```

---

*Source: `ComOff/LaunchLabVIEW.htm`*
