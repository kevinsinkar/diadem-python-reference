---
title: "PathAddTrailingBackslash"
description: "Adds a trailing backslash \\ to a path. The path then fulfils the DIAdem requirements. If the path already ends with a backslash, DIAdem does not add a second ba"
---

# PathAddTrailingBackslash

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PathAddTrailingBackslash

Adds a trailing backslash \ to a path. The path then fulfils the DIAdem requirements. If the path already ends with a backslash, DIAdem does not add a second backslash.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">InputPath</td>
<td>Suggests a path.<div id="exp_InputPath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String</a> type.</td></tr>
</table>
</div>

## Python example

```python
print(dd.PathAddTrailingBackslash("d:\\Test")) #=> "d:\Test\"
print(dd.PathAddTrailingBackslash("d:\\Test\\")) #=> "d:\Test\"
```

---

*Source: `ComOff/PathAddTrailingBackslash.htm`*
