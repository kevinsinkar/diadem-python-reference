---
title: "LoopDeInit"
description: "Ends a progress bar display in the status bar. Use the LoopInit command to initialize the progress bar display in the status bar."
---

# LoopDeInit

!!! abstract "Command &middot; `ComOff.chm`"
    Command: LoopDeInit

Ends a progress bar display in the status bar. Use the LoopInit command to initialize the progress bar display in the status bar.

## Signature

```python
dd.LoopDeInit()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>While controlling the progress display with the <span class="Monospace">LoopInc</span> command, DIAdem suppresses the progress display of other DIAdem commands.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Python example

```python
dd.LoopInit()
for intLoop in range( 1, 100+1):
    dd.LoopInc(intLoop)
    dd.Pause(0.1)
dd.LoopDeInit()
```

---

*Source: `ComOff/LoopDeInit.htm`*
