---
title: "UnEscapeDatastring"
description: "Decodes the texts encoded with the EscapeDataString command."
---

# UnEscapeDatastring

!!! abstract "Command &middot; `ComOff.chm`"
    Command: UnEscapeDatastring

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('UrlDataString', ...)   # instead of dd.UrlDataString = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Decodes the texts encoded with the EscapeDataString command.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">URLEscapedDataString</td>
<td>Specifies the text to be decoded<div id="exp_URLEscapedDataString">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String</a> type. Receives the decoded text.</td></tr>
</table>
</div>

## Python example

```python
dd.UrlDataString = "abcde :// ????????"

dd.UrlEscapedDataString = dd.EscapeDataString(dd.UrlDataString)
dd.LogfileWrite(dd.UrlEscapedDataString)

dd.UrlDataString = dd.UnescapeDataString(dd.UrlEscapedDataString)
dd.LogfileWrite(dd.UrlDataString)
```

---

*Source: `ComOff/UnEscapeDatastring.htm`*
