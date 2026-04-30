---
title: "MKSCheck"
description: "Checks the definitions and the connections of the loaded block diagram."
---

# MKSCheck

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: MKSCheck

Checks the definitions and the connections of the loaded block diagram.

## Signature

```python
dd.MKSCheck([DHI1])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the <a href="../schemecheck/">SchemeCheck</a> command and then the <span class="Monospace">MKSCheck</span> command, for a complete block diagram check.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[DHI1]</td>
<td>For future extensions.</td></tr>
</table>
</div>

## Python example

```python
dd.SchemeLoad("Example")
dd.SchemeCheck("Normal")
dd.MKSCheck(0)
```

---

*Source: `ComOnl/MKSCheck.htm`*
