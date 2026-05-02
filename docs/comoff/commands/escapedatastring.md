---
title: "EscapeDatastring"
description: "Encodes a text using the URL encoding so that the string can be used as a parameter in a URL. With the exception of letters, numbers, and a few special characte"
---

# EscapeDatastring

!!! abstract "Command &middot; `ComOff.chm`"
    Command: EscapeDatastring

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('UrlDataString', ...)   # instead of dd.UrlDataString = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Encodes a text using the URL encoding so that the string can be used as a parameter in a URL. With the exception of letters, numbers, and a few special characters, the command replaces each byte of the characters passed with a percent sign and two hexadecimal digits. Do not use this command to encode entire URLs, because the command also encodes the characters "/" and ":".

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">URLDataString</td>
<td>Specifies the text to be encoded.<div id="exp_URLDataString">
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
<td>The return value is a <a href="#" data-unresolved="1">String</a> type. Receives the encoded text.</td></tr>
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

*Source: `ComOff/EscapeDatastring.htm`*
