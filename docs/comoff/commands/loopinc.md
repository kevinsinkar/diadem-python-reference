---
title: "LoopInc"
description: "Modifies the percentage of the progress bar in the status bar. For example, if you assign the value 50 to the LoopLength parameter, DIAdem shows only half of th"
---

# LoopInc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: LoopInc

Modifies the percentage of the progress bar in the status bar. For example, if you assign the value 50 to the LoopLength parameter, DIAdem shows only half of the progress bar. Use the LoopInit command to initialize the progress bar and the LoopDeInit command to terminate the progress bar.

## Signature

```python
dd.LoopInc(LoopLength)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>While controlling the progress display with the <span class="Monospace">LoopInc</span> command, DIAdem suppresses the progress display of other DIAdem commands.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">LoopLength</td>
<td>Specifies the percentage of the progress bar in the status bar. Valid values range between 1 and 100.<div id="exp_LoopLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
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

*Source: `ComOff/LoopInc.htm`*
