---
title: "PathExpand"
description: "Changes a relative path into an absolute path. The input path can contain \".\", \"..\", \"/\" and \"\\\". The command does not check whether the path exists."
---

# PathExpand

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PathExpand

Changes a relative path into an absolute path. The input path can contain ".", "..", "/" and "\". The command does not check whether the path exists.

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
dd.T1 = dd.CurrentScriptPath + "..\\Subfolder\\MyFile.VBS"
dd.T2 = dd.PathExpand(dd.T1)
print(dd.T1 + "\r\n" + "=>" + "\r\n" + dd.T2)
dd.T1 = dd.CurrentScriptPath + "..\\Subfolder\\.\\MyFile.VBS"
dd.T2 = dd.PathExpand(dd.T1)
print(dd.T1 + "\r\n" + "=>" + "\r\n" + dd.T2)
dd.T1 = "..\\Subfolder\\MyFile.VBS"
dd.T2 = dd.PathExpand(dd.T1)
print(dd.T1 + "\r\n" + "=>" + "\r\n" + dd.T2)
dd.T1 = ".\\Subfolder\\MyFile.VBS"
dd.T2 = dd.PathExpand(dd.T1)
print(dd.T1 + "\r\n" + "=>" + "\r\n" + dd.T2)
dd.T1 = "./Subfolder/MyFile.VBS"
dd.T2 = dd.PathExpand(dd.T1)
print(dd.T1 + "\r\n" + "=>" + "\r\n" + dd.T2)
```

---

*Source: `ComOff/PathExpand.htm`*
