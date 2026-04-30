---
title: "ODS_UploadFilesToBlob"
description: "Loads files as a DT_Blob type attribute onto an ASAM ODS CORBA server."
---

# ODS_UploadFilesToBlob

!!! abstract "Function &middot; `ComOff.chm`"
    Function: ODS_UploadFilesToBlob

Loads files as a DT_Blob type attribute onto an ASAM ODS CORBA server.

## Signature

```python
ReturnValue = ODS_UploadFiles(Store, Instance, PropertyName, BlobHeader, UploadFileName)
```

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
dd.ScriptInclude(dd.ProgramDrv + "Libr\\Documents\\Utils\\ODS\\UploadFiles.vbs")
StoreType = "AOP5"
StoreParam = "<corba>corbaname::10.89.2.24:900/NameService#org/asam/ods/ENGINE1</corba><user>System</user><pwd e=\"1\" c=\"0\">puma</pwd>"
InstanceKey = "ParameterFile 1"
PropertyName = "iFile"
Store = dd.Navigator.ConnectDataStoreByParameter(StoreType, StoreParam)
Instance = Store.GetElementByKey(InstanceKey)
SourceFile = dd.TmpDrv + "Layout.tdr"
rc = ODS_UploadFiles_ToBlob(Store, Instance, PropertyName, "DIAdem layout for reporting", SourceFile)
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

*Source: `ComOff/ODS_UploadFiles.htm`*
