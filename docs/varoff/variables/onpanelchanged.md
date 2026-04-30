---
title: "OnPanelChanged"
description: "Specifies the command that DIAdem executes when DIAdem switches to another DIAdem panel."
---

# OnPanelChanged

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: OnPanelChanged

Specifies the command that DIAdem executes when DIAdem switches to another DIAdem panel.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to <a href="#" data-unresolved="1">Working with Events in DIAdem</a> for further information.</td></tr></table>
</div>

## Python example

```python
def MyModul(LastPanel, NewPanel):
    dd.MsgBoxDisp("Deactivate: "  + LastPanel + "; Activate: " + NewPanel)
```

---

*Source: `VarOff/OnPanelChanged.htm`*
