---
title: "OLEInterfaceLock"
description: "Blocks or opens the OLE interfaces TOCommand and TODataSheet ."
---

# OLEInterfaceLock

!!! abstract "Command &middot; `ComOff.chm`"
    Command: OLEInterfaceLock

Blocks or opens the OLE interfaces TOCommand and TODataSheet .

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OLELockMode</td>
<td>Specifies the status of the OLE interfaces <a href="../../../ole/objects/itocommand/">TOCommand</a> and <a href="../../../ole/objects/itodatasheet/">TODataSheet</a>.<div id="exp_OLELockMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"OLEUnlockAll"</pre></donottranslate></td>
<td>Unlocks all OLE interfaces</td></tr>
<tr><td width="150"><donottranslate><pre>"OLELockCommand"</pre></donottranslate></td>
<td>Locks the OLE interface TOCommand</td></tr>
<tr><td width="150"><donottranslate><pre>"OLELockDatasheet"</pre></donottranslate></td>
<td>Locks the OLE interface TODataSheet</td></tr>
<tr><td width="150"><donottranslate><pre>"OLELockAll"</pre></donottranslate></td>
<td>Locks all OLE interfaces</td></tr>
<tr><td width="150"><donottranslate><pre>"OLEGetLockInfo"</pre></donottranslate></td>
<td>Requests the status of the OLE interfaces</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the status of the OLE interfaces <a href="../../../ole/objects/itocommand/">TOCommand</a> and <a href="../../../ole/objects/itodatasheet/">TODataSheet</a>. The return value is a OLELockMode type.<div id="exp_OLELockMode__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"OLEUnlockAll"</pre></donottranslate></td>
<td>Unlocks all OLE interfaces</td></tr>
<tr><td width="150"><donottranslate><pre>"OLELockCommand"</pre></donottranslate></td>
<td>Locks the OLE interface TOCommand</td></tr>
<tr><td width="150"><donottranslate><pre>"OLELockDatasheet"</pre></donottranslate></td>
<td>Locks the OLE interface TODataSheet</td></tr>
<tr><td width="150"><donottranslate><pre>"OLELockAll"</pre></donottranslate></td>
<td>Locks all OLE interfaces</td></tr>
<tr><td width="150"><donottranslate><pre>"OLEGetLockInfo"</pre></donottranslate></td>
<td>Requests the status of the OLE interfaces</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/OLEInterfaceLock.htm`*
