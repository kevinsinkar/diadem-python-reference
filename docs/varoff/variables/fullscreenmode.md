---
title: "FullScreenMode"
description: "Receives the information whether DIAdem displays in the full-screen mode or in the standard size. This variable is read only. To switch the full screen mode on "
---

# FullScreenMode

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: FullScreenMode

Receives the information whether DIAdem displays in the full-screen mode or in the standard size. This variable is read only. To switch the full screen mode on or off, use the WndShow command.

## Python example

```python
dd.MsgBoxDisp("DIAdem is displayed in this mode: " + dd.FullScreenMode)
dd.WndShow("SHELL","FULLSIZE")
dd.MsgBoxDisp("DIAdem is displayed in this mode: " + dd.FullScreenMode)
dd.MsgBoxDisp("Press <CTRL-U> to exit fullsize mode")
```

---

*Source: `VarOff/FullScreenMode.htm`*
