---
title: "GlobalFnScriptGet"
description: "Returns the script that is assigned to a button of the global script bar."
---

# GlobalFnScriptGet

!!! abstract "Function &middot; `ComOff.chm`"
    Function: GlobalFnScriptGet

Returns the script that is assigned to a button of the global script bar.

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

## Returns

<div markdown="1">
<table class="Borderless" id="table2">
<tr><td width="150"><em>PathFile</em></td>
<td>Receives the name of the script file to be executed, including the path. If no script is assigned to the button, the function returns an empty text.<div id="exp_PathFile"><a href="#" data-unresolved="1">String variable</a></div></td></tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp(GlobalFnScriptGet(2))
```

---

*Source: `ComOff/GlobalFnScriptGet.htm`*
