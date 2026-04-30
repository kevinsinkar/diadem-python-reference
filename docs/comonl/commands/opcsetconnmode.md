---
title: "OPCSetConnMode"
description: "Specifies when DIAdem starts OPC servers and when DIAdem stops OPC servers."
---

# OPCSetConnMode

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetConnMode

Specifies when DIAdem starts OPC servers and when DIAdem stops OPC servers.

## Signature

```python
dd.OPCSetConnMode(OPCConnMode)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the <span class="Monospace">OPCConnMode</span> variable has the value <span class="Monospace">2</span>, DIAdem can terminate the loading of a block diagram, if DIAdem cannot establish a connection to the OPC servers that are referenced in the block diagram.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCConnMode</td>
<td>Specifies the start settings and stop settings for OPC servers.<div id="exp_OPCConnMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCConnMode &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCConnMode</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>DIAdem starts all OPC servers as soon as a block diagram establishes communication to an OPC server, and maintains the connection.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>DIAdem ends all OPC servers after a measurement or configuration.</td></tr><tr><td width="150"><pre><donottranslate>2</donottranslate></pre></td><td>DIAdem starts all OPC servers as soon as a block diagram contains a reference to an OPC server, and maintains the connection.</td></tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetConnMode.htm`*
