---
title: "UnEscapeDatastring"
description: "Decodes the texts encoded with the EscapeDataString command."
---

# UnEscapeDatastring

!!! abstract "Command &middot; `ComOff.chm`"
    Command: UnEscapeDatastring

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
