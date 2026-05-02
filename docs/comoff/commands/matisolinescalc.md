---
title: "MatIsolinesCalc"
description: "Calculates contour lines on a surface with a matrix."
---

# MatIsolinesCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatIsolinesCalc

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('D3IsoLineSource', ...)   # instead of dd.D3IsoLineSource = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Calculates contour lines on a surface with a matrix.

## Signature

```python
dd.MatIsolinesCalc( X , Y , ChnList)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The value of the variable <span class="Monospace">HullFactor</span> should not be greater than the value of the variable <a href="../../../varoff/variables/hulltol/">HullTol</a> that specifies the maximum edge length of the hull.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You only can use the <span class="Monospace">D3IsolineBdry</span> variable if the input data have a matrix structure.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem saves the associated contour value in the <span class="Monospace">ResultIsovalue</span> custom property of the respective result channel.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("Grp/ChnZ*")
dd.D3IsoLineSource ="calculated"
dd.D3IsoLineCalc ="automatic"
dd.D3IsoLineBDry =0
dd.MatIsolinesCalc("Grp/ChnX", "Grp/ChnY", oMyChannelList)
```

---

*Source: `ComOff/MatIsolinesCalc.htm`*
