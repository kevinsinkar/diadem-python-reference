---
title: "CTNV"
description: "Converts a Boolean expression to NoValue or to 0 ."
---

# CTNV

!!! abstract "Function &middot; `ComOff.chm`"
    Function: CTNV

Converts a Boolean expression to NoValue or to 0 .

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>bConditionValue</em></td>
<td>Specifies the expression to be checked.<div id="exp_bCondionValue"><a href="#" data-unresolved="1">Boolean variable</a></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>If the expression in <em><span class="Monospace">bCondionValue</span></em> is TRUE, the function receives <a href="#" data-unresolved="1">NoValue</a> as the return value, otherwise it receives <span class="Monospace">0</span>.</td></tr>
</table>
</div>

## Python example

```python
dd.Calculate("Ch(\"Group2/Result\") = Ch(\"[1]/[2]\")*(1+CTNV(Ch(\"[1]/[2]\")>10))")
```

---

*Source: `ComOff/CTNV.htm`*
