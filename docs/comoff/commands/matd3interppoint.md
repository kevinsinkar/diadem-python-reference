---
title: "MatD3InterpPoint"
description: "Calculates a single z-value of a three-dimensional interpolation for an x-channel, a y-channel, and a z-matrix."
---

# MatD3InterpPoint

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatD3InterpPoint

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.IntegerVarSet('D3GridCalcAll', ...)   # instead of dd.D3GridCalcAll = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Calculates a single z-value of a three-dimensional interpolation for an x-channel, a y-channel, and a z-matrix.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the variables <a href="../../../varoff/variables/d3gridpolyg/">D3GridPolyg</a>, <a href="../../../varoff/variables/d3gridpolygchn/">D3GridPolygChn</a>, and <a href="../../../varoff/variables/d3gridpolygconv/">D3GridPolygConv</a> to specify the section.</td></tr></table>
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
<tr><td width="150">Value</td>
<td>Specifies the x-value for the point at which DIAdem calculates the z-value.<div id="exp_Value">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">Value</td>
<td>Specifies the y-value for the point at which DIAdem calculates the z-value.<div id="exp_Value__1">
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
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Floating-point number</a> type.</td></tr>
</table>
</div>

## Python example

```python
oMyChannelList = dd.Data.GetChannels("Grp/ChnZ*")
dd.D3GridCalcAll =0
dd.D3GridPolyg ="convex hull"
z = dd.MatD3InterpPoint("Grp/ChnX", "Grp/ChnY", oMyChannelList, 1.23, 4.56)
```

---

*Source: `ComOff/MatD3InterpPoint.htm`*
