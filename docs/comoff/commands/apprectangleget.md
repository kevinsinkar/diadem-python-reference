---
title: "AppRectangleGet"
description: "Specifies the size of a DIAdem window area. DIAdem returns a zero based array which contains the distance in pixels from the left, the upper, the right, and the"
---

# AppRectangleGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AppRectangleGet

Specifies the size of a DIAdem window area. DIAdem returns a zero based array which contains the distance in pixels from the left, the upper, the right, and the lower edge to the screen origin. The screen origin is the top-left corner of the screen.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AppRectangleType</td>
<td>Specifies the window area of DIAdem. The value 0 corresponds to the DIAdem main window or the value 1 corresponds to the area below the last symbol of the panel bar.<div id="exp_AppRectangleType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AppRectangleType &lt;= 1</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant variable</a> type. DIAdem returns a zero-based array that contains the distance. If the panel bar is not visible or does not exist and the command is called with the value <span class="Monospace">1</span>, the function returns NULL.</td></tr>
</table>
</div>

## Python example

```python
iFreeBarRect = dd.AppRectangleGet(1)
if not iFreeBarRect == None :
    dd.MsgBoxDisp("Left: " + iFreeBarRect(0) + ", Top: " + iFreeBarRect(1) + ", Right: " + iFreeBarRect(2) + ", Bottom: " + iFreeBarRect(3))
else:
    dd.MsgBoxDisp("There is no visible panel bar")
```

---

*Source: `ComOff/AppRectangleGet.htm`*
