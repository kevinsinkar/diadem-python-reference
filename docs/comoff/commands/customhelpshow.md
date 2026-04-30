---
title: "CustomHelpShow"
description: "Opens a user-defined help file in the CHM format."
---

# CustomHelpShow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CustomHelpShow

Opens a user-defined help file in the CHM format.

## Signature

```python
dd.CustomHelpShow(CustomHelpFilename, CustomHelpURL)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Use the text <span class="Monospace">custom_main</span> as the <span class="Monospace">Window type</span> so that DIAdem displays the user-defined help files correctly. Specify the window definition in the HHP file and in the HHK file.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CustomHelpFilename</td>
<td>Specifies the name of a help file.<div id="exp_CustomHelpFilename">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">CustomHelpURL</td>
<td>Specifies the URL of the help page.<div id="exp_CustomHelpURL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.CustomHelpShow("Customize.chm","Customize.chm::/Page1.htm")
```

---

*Source: `ComOff/CustomHelpShow.htm`*
