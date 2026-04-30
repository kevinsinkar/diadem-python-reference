---
title: "SchemeLoad"
description: "Loads a block diagram."
---

# SchemeLoad

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: SchemeLoad

Loads a block diagram.

## Signature

```python
dd.SchemeLoad(SchemeFile)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SchemeFile</td>
<td>Specifies the name of the current block diagram.<div id="exp_SchemeFile">
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
dd.SchemeLoad("Example")
dd.SchemeCheck("Normal")
dd.SchemeMeasTest()
```

---

*Source: `ComOnl/SchemeLoad.htm`*
