---
title: "SchemeCheck"
description: "Transfers a block diagram into the measurement kernel and checks this block diagram."
---

# SchemeCheck

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: SchemeCheck

Transfers a block diagram into the measurement kernel and checks this block diagram.

## Signature

```python
dd.SchemeCheck(SchemeCheckMsg)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SchemeCheckMsg</td>
<td>Specifies whether DIAdem displays messages after checking a block diagram.<div id="exp_SchemeCheckMsg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"normal"</pre></donottranslate></td>
<td>Normal</td></tr>
<tr><td width="150"><donottranslate><pre>"no Message"</pre></donottranslate></td>
<td>No message</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.SchemeLoad("Example")
dd.SchemeCheck("Normal")
dd.SchemeMeasTest()
```

---

*Source: `ComOnl/SchemeCheck.htm`*
