---
title: "CClassXRedXY"
description: "Classifies a signal and reduces the result data."
---

# CClassXRedXY

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CClassXRedXY

Classifies a signal and reduces the result data.

## Signature

```python
dd.CClassXRedXY( X , X1 , Y , ClassMeth2, ClassXRed, ClassDontUseNV, ClassNVReplace)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel that contains the x-values.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel that contains the x1-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values.</td></tr>
<tr><td width="150">ClassMeth2</td>
<td>Specifies how DIAdem specifies the class limits.<div id="exp_ClassMeth2">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginEnd"</pre></donottranslate></td>
<td>Number/Begin/End</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginWidth"</pre></donottranslate></td>
<td>Number/Begin/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginRange"</pre></donottranslate></td>
<td>Number/Begin/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"NoEndWidth"</pre></donottranslate></td>
<td>Number/End/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"NoEndRange"</pre></donottranslate></td>
<td>Number/End/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"BeginEndWidth"</pre></donottranslate></td>
<td>Begin/End/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"BeginWidthRange"</pre></donottranslate></td>
<td>Begin/Width/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"EndWidthRange"</pre></donottranslate></td>
<td>End/Width/Range</td></tr>
</table>
</td></tr>
</table>
<p class="Body">When you use the <span class="Monospace">Automatic</span> method, you specify the number of classes. DIAdem calculates the missing parameters from the maximum and minimum values of the channel to be classified.</p>
</div></td></tr>
<tr><td width="150">ClassXRed</td>
<td>Specifies the type of data reduction.<div id="exp_ClassXRed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Mean"</pre></donottranslate></td>
<td>Mean value</td></tr>
<tr><td width="150"><donottranslate><pre>"minimum"</pre></donottranslate></td>
<td>Minimum</td></tr>
<tr><td width="150"><donottranslate><pre>"maximum"</pre></donottranslate></td>
<td>Maximum</td></tr>
<tr><td width="150"><donottranslate><pre>"Sum"</pre></donottranslate></td>
<td>Sum</td></tr>
<tr><td width="150"><donottranslate><pre>"Quantity"</pre></donottranslate></td>
<td>Number of</td></tr>
</table>
</td></tr>
</table><strong><p class="Body">Valid settings</p></strong><table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" id="AutoNumber1" style="border-collapse: collapse" width="619">
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">Mean</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem averages the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">minimum</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem averages the minimum of all the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">maximum</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem averages the maximum of all the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">Sum</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem totals all the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">Quantity</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem specifies the number of y-values of a class.</p>
</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ClassDontUseNV</td>
<td>Specifies whether DIAdem ignores or replaces <a href="../../../varoff/variables/nv/">NoValues</a> in a reducing classification. The default value is <span class="Monospace">FALSE</span> which specifies that DIAdem does not replace NoValues.<div id="exp_ClassDontUseNV">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ClassNVReplace</td>
<td>Specifies the value with which DIAdem replaces NoValues in a reducing classification. The default value of the <span class="Monospace">ClassNVReplace</span> variable is <span class="Monospace">0</span>.<div id="exp_ClassNVReplace">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/CClassXRedXY.htm`*
