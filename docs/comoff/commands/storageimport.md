---
title: "StorageImport"
description: "Loads data from an external server-based data store into the DIAdem Data Portal."
---

# StorageImport

!!! abstract "Command &middot; `ComOff.chm`"
    Command: StorageImport

Loads data from an external server-based data store into the DIAdem Data Portal.

## Signature

```python
return_value = dd.StorageImport(StorageABS, [ImportParameterSet])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you use the <span class="Monospace">ImportParameter</span> object for the <span class="Monospace">ImportParameterSet</span> parameter, the <span class="Monospace">StorageImport</span> command only supports the properties:<a href="../../../scriptnavi/properties/iimportparameterset-importmode/">ImportMode</a> and <a href="../../../scriptnavi/properties/iimportparameterset-loadreturnmode/">LoadReturnMode</a>. The command ignores all other properties.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The <span class="Monospace">StorageABS</span> variable displays a key as an XML string that you can use to access external data stores. If you load channels from an external data store in the recording mode, DIAdem usually records the key.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">StorageABS</td>
<td>Specifies a key that you can use to access external data stores.<div id="exp_StorageABS">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If you load channels from an external data store, the key is often in the <span class="Monospace">Origin key</span> property of the channel.</p>
</div></td></tr>
<tr><td width="150">[ImportParameterSet]</td>
<td>Specifies how DIAdem imports data into the Data Portal. Use the <a href="../../../scriptnavi/objects/iimportparameterset/">ImportParameter</a> object for the <span class="Monospace">ImportParameterSet</span> parameter. You can also use one of the following script terms as an alternative.<div id="exp_ImportParameterSet">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless">
<tr>
<td><table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Load"</pre></donottranslate></td>
<td>Load</td></tr>
<tr><td width="150"><donottranslate><pre>"Load|ChnXYRelation"</pre></donottranslate></td>
<td>Load with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"Register"</pre></donottranslate></td>
<td>Register</td></tr>
<tr><td width="150"><donottranslate><pre>"Register|ChnXYRelation"</pre></donottranslate></td>
<td>Login with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"Append"</pre></donottranslate></td>
<td>Append</td></tr>
<tr><td width="150"><donottranslate><pre>"Append|ChnXYRelation"</pre></donottranslate></td>
<td>Append with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadImmediately"</pre></donottranslate></td>
<td>Always load bulk data</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadImmediately|ChnXYRelation"</pre></donottranslate></td>
<td>Always load bulk data with x-channel reference</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnFirstAccess"</pre></donottranslate></td>
<td>Load bulk data on first access</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnFirstAccess|ChnXYRelation"</pre></donottranslate></td>
<td>Load bulk data with x-channel reference on first access</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnWriteAccess"</pre></donottranslate></td>
<td>Load bulk data when writing channel data</td></tr>
<tr><td width="150"><donottranslate><pre>"LoadOnWriteAccess|ChnXYRelation"</pre></donottranslate></td>
<td>Load bulk data with x-channel reference when writing channel data</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td><a href="../../../scriptnavi/collections/elementlist-2/">ElementList &lt;Data&gt; object</a> type return value.<br attr="ext"/>Element list with the elements. Use the <a href="../../../scriptnavi/properties/iimportparameterset-loadreturnmode/">LoadReturnMode</a> property to specify which elements the element list contains.</td></tr>
</table>
</div>

---

*Source: `ComOff/StorageImport.htm`*
