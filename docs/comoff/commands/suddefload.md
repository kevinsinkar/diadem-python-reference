---
title: "SUDDefLoad"
description: "Specifies a SUD file that contains one or more user dialog boxes."
---

# SUDDefLoad

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SUDDefLoad

Specifies a SUD file that contains one or more user dialog boxes.

## Signature

```python
dd.SUDDefLoad(SUDFileName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Always use the <span class="Monospace">SUDDefLoad</span> command with the <a href="../suddlgshow/">SudDlgShow</a> command. The <span class="Monospace">SudDlgShow</span> command displays a user dialog box.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
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

## Python example

```python
dd.SUDDefLoad("Example.sud")
dd.SUDDlgShow("Dialog1")
```

---

*Source: `ComOff/SUDDefLoad.htm`*
