---
title: "ChnIntegrate"
description: "Integrates a signal."
---

# ChnIntegrate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnIntegrate

Integrates a signal.

## Signature

```python
return_value = dd.ChnIntegrate( XW , Y , ResultChannel , [IntegrationMethod], [IntegrationConstant], [IntegrationConstantManual], [IntegrationFinalValue])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel with the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel with the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the name of the result channel.</td></tr>
<tr><td width="150">[IntegrationMethod]</td>
<td>Specifies the integration method.<div id="exp_IntegrationMethod">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"TrapezoidalRule"</pre></donottranslate></td>
<td>Trapezoidal rule</td></tr>
<tr><td width="150"><donottranslate><pre>"SimpsonRule"</pre></donottranslate></td>
<td>Simpson rule</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[IntegrationConstant]</td>
<td>Specifies the constant, which DIAdem adds to the integral after the integration.<div id="exp_IntegrationConstant">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[IntegrationConstantManual]</td>
<td>Specifies whether DIAdem uses an integration constant for the trapezoidal rule. Do not enable this option if you want to continue calculating with the method valid up to version 2012. The integration constant is always used with the Simpson rule.<div id="exp_IntegrationConstantManual">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[IntegrationFinalValue]</td>
<td>Specifies the integration end value according to the Simpson rule.<div id="exp_IntegrationFinalValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnIntegrate.htm`*
