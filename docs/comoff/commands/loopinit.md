---
title: "LoopInit"
description: "Initializes the progress bar with a percentage in the status bar. Use the LoopInc command to change the value of the progress bar."
---

# LoopInit

!!! abstract "Command &middot; `ComOff.chm`"
    Command: LoopInit

Initializes the progress bar with a percentage in the status bar. Use the LoopInc command to change the value of the progress bar.

## Signature

```python
dd.LoopInit()
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

*Source: `ComOff/LoopInit.htm`*
