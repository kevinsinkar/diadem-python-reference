---
title: "IIf"
description: "Provides an If-Then-Else-EndIf expression in one line and returns one of the transferred parameters dependent on the evaluation of the expression."
---

# IIf

!!! abstract "Function &middot; `ComOff.chm`"
    Function: IIf

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.BoolVarSet('CalcQuantityBased', ...)   # instead of dd.CalcQuantityBased = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Provides an If-Then-Else-EndIf expression in one line and returns one of the transferred parameters dependent on the evaluation of the expression.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>If you use the function IIF together with the <span class="Monospace">Calculate</span> command and enable quantity-based calculation, DIAdem sometimes converts the channel units into a different unit. Use the <span class="Monospace">VU</span> function for the constant comparison, in order to assign a unit to the constant. Refer to the help page of the <a href="../../commands/calculate/">Calculate</a> command and the <a href="#" data-unresolved="1">VU</a> function for further information.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>bConditionValue</em></td>
<td>Specifies the expression to be checked.<div id="exp_bCondionValue"><a href="#" data-unresolved="1">Boolean variable</a></div></td></tr>
<tr><td width="150"><em>vTrueValue</em></td>
<td>Specifies the parameter that DIAdem returns when the expression is <span class="Monospace">TRUE</span>.<div id="exp_vTrueValue"><a href="#" data-unresolved="1">Variant variable</a></div></td></tr>
<tr><td width="150"><em>vFalseValue</em></td>
<td>Specifies the parameter that DIAdem returns when the expression is <span class="Monospace">FALSE</span>.<div id="exp_vFalseValue"><a href="#" data-unresolved="1">Variant variable</a></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Depending on the evaluation of the expression in <em><span class="Monospace">bCondionValue</span></em>, the function receives the return value <em>vTrueValue</em> or<em> vFalseValue</em>.</td></tr>
</table>
</div>

## Python example

```python
iInput = dd.InputBoxDisp ("Enter a value")
dd.MsgBoxDisp (IIf(iInput>5, "Input value > 5", "Input value <= 5"))
```

```python
dd.CalcQuantityBased = True
dd.Calculate("Ch(\"ResultNV\")=IIf( Ch(\"Temperatur_1\")<VU(28,\"+deg;C\"),Ch(\"Temperatur_1\"),NoValue)")
```

```python
dd.Calculate("Ch(\"ResultNeg\")=IIf( Ch(\"ResultNV\") == None,-1,Ch(\"ResultNV\"))")
```

---

*Source: `ComOff/IIF.htm`*
