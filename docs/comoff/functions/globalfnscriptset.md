---
title: "GlobalFnScriptSet"
description: "Assigns a script to a button of the global script bar."
---

# GlobalFnScriptSet

!!! abstract "Function &middot; `ComOff.chm`"
    Function: GlobalFnScriptSet

Assigns a script to a button of the global script bar.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note</strong>  The command replaces the AutoIconSet command.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless" id="table1">
<tr><td width="150"><em>Key</em></td>
<td>Specifies the function keys F1 to F12.<div id="exp_key"><a href="#" data-unresolved="1">Integer variable</a><table class="Borderless" id="table3">
<tr>
<td>1 &lt;= Key &lt;= 12</td>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
GlobalFnScriptSet(2, dd.ScriptReadPath + "MyScript.vbs")
```

---

*Source: `ComOff/GlobalFnScriptSet.htm`*
