---
title: "CPUAffinitySet"
description: "Specifies which processors DIAdem uses in a multiprocessor environment."
---

# CPUAffinitySet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CPUAffinitySet

Specifies which processors DIAdem uses in a multiprocessor environment.

## Signature

```python
dd.CPUAffinitySet(CPUAffinity)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CPUAffinity</td>
<td>Receives the names of the processors that DIAdem uses.<div id="exp_CPUAffinity">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">Every bit of the variable represents a processor (CPU). For example, if the variable contains the decimal value <span class="Monospace">3</span>, DIAdem uses the first and the second processor, because the bit sequence <span class="Monospace">11</span> corresponds to the decimal value <span class="Monospace">3</span>.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/CPUAffinitySet.htm`*
