---
title: "ODS_GetMultipleChildren"
description: "Returns all referenced elements of a base type in an ASAM data store."
---

# ODS_GetMultipleChildren

!!! abstract "Function &middot; `ComOff.chm`"
    Function: ODS_GetMultipleChildren

Returns all referenced elements of a base type in an ASAM data store.

## Signature

```python
ReturnValue = ODS_GetMultipleChildren(Store, Instance)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You must include the <span class="Monospace">ODS_GetMultipleChildren</span> library in your script in order to be able to use the <span class="Monospace">GetMultipleChildren.vbs</span> command.</td></tr></table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150"><em>ReturnValue</em></td>
<td>Receives a field which contains the list of referenced elements. If no element is referenced, the command returns <span class="Monospace">Empty</span>.</td>
</tr>
</table>
</div>

## Python example

```python
#Load the ODS supporting library
dd.ScriptInclude(dd.ProgramDrv + "Libr\\Documents\\Utils\\ODS\\GetMultipleChildren.vbs")
sAtfxFilePath = dd.ProgramDrv + "Examples\\Data\\ASAMMultipleChildren.atfx"
sOpenParameter = "\"" + Replace(sAtfxFilePath.replace( "+", "+amp;"), "<",  "<") + "\""
# Open store containing ASAM model with multiple children like openMDM model
oStore = dd.Navigator.ConnectDataStoreByParameter("ATFX", sOpenParameter)

# Get an instance of type aomeasurement
oMeaCollection = oStore.GetElementList("MeaResult", "", False)
oMea = oMeaCollection.Item(1)

# Retrieve the related oUut and its parts
oUutCollection = oMea.References.Item("units_under_test").Elements
oUut = oUutCollection.Item(1)
aUutParts = ODS_GetMultipleChildren(oStore, oUut)
# The result is a vbs array containing the related elements

# Retrieve the related oSequence and its parts
oSequenceCollection = oMea.References.Item("sequences").Elements
oSequence = oSequenceCollection.Item(1)
aSequenceParts = ODS_GetMultipleChildren(oStore, oSequence)

# Retrieve the related oEquipment and its parts
oEquipmentCollection = oMea.References.Item("equipments").Elements
oEquipment = oEquipmentCollection.Item(1)
aEquipmentParts = ODS_GetMultipleChildren(oStore, oEquipment)

# Retrieve "name" attribute of oUut and its parts
sOutput = sOutput + "  " + oUut.Type + ": " + oUut.Name + "\r\n"
for oUutPart in aUutParts:
    sOutput = sOutput + "      " + oUutPart.Type + ": " + oUutPart.Name + "\r\n"
# Retrieve "name" attribute of oEquipment and its parts
sOutput = sOutput + "  " + oEquipment.Type + ": " + oEquipment.Name + "\r\n"
for oEquipmentPart in aEquipmentParts:
    sOutput = sOutput + "      " + oEquipmentPart.Type + ": " + oEquipmentPart.Name + "\r\n"
# Retrieve "name" attribute of oSequence and its parts
sOutput = sOutput + "  " + oSequence.Type + ": " + oSequence.Name + "\r\n"
for sequencePart in aSequenceParts:
    sOutput = sOutput + "      " + sequencePart.Type + ": " + sequencePart.Name + "\r\n"

print(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<p></p><table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You must include the <span class="Monospace">ODS_GetMultipleChildren</span> library in your script in order to be able to use the <span class="Monospace">GetMultipleChildren.vbs</span> command.</td></tr></table>
<h2>See Also</h2>
<p class="body"><a href="../../../tdmscript/objects/idatafileheader/">DataFileHeader</a></p>
</div>
</div>

---

*Source: `ComOff/ODS_GetMultipleChildren.htm`*
