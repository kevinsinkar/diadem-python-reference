---
title: "ODS_DownloadFiles"
description: "Loads binary file from an ASAM ODS CORBA server."
---

# ODS_DownloadFiles

!!! abstract "Function &middot; `ComOff.chm`"
    Function: ODS_DownloadFiles

Loads binary file from an ASAM ODS CORBA server.

## Signature

```python
ReturnValue = ODS_DownloadFiles(Store, Instance, PropertyName, DownloadFileName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">ODS_DownloadFiles</span> function does not create new folders. If a file already exists with the specified name, the function overwrites this file.</td></tr></table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150"><em>ReturnValue</em></td>
<td>Returns the value 0 if the function was executed successfully. Displays an error if the input is invalid.</td>
</tr>
</table>
</div>

## Python example

```python
dd.ScriptInclude(dd.ProgramDrv + "Libr\\Documents\\Utils\\ODS\\DownloadFiles.vbs")
StoreType = "AOP5"
StoreParam = "<corba>corbaname::10.89.2.24:900/NameService#org/asam/ods/ENGINE1</corba><user>System</user><pwd e=\"1\" c=\"0\">puma</pwd>"
InstanceKey = "ParameterFile 1"
PropertyName = "iFile"
Store = dd.Navigator.ConnectDataStoreByParameter(StoreType, StoreParam)
Instance = Store.GetElementByKey(InstanceKey)
TargetFile = dd.TmpDrv + "_Target.bin"
rc = ODS_DownloadFiles(Store, Instance, PropertyName, TargetFile)
print(rc)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="../../../tdmscript/objects/idatafileheader/">DataFileHeader</a></p>
</div>
</div>

---

*Source: `ComOff/ODS_DownloadFiles.htm`*
