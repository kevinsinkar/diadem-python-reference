---
title: "CreateDataFileHeaderAccess"
description: "By creating a DataFileHeaderAccess object , provides access to a data store with which you read, write, change, and delete the channel properties, group propert"
---

# CreateDataFileHeaderAccess

!!! abstract "Function &middot; `ComOff.chm`"
    Function: CreateDataFileHeaderAccess

By creating a DataFileHeaderAccess object , provides access to a data store with which you read, write, change, and delete the channel properties, group properties, and root properties of files, whereby the associated mass data is write-protected. For full access to a data store, use the DataStoreDisplay . GetDataStore , the Navigator . ConnectDataStore , or the Navigator . ConnectDataStoreByParameter method.

## Signature

```python
value = dd.CreateDataFileHeaderAccess
```

## Python example

```python
oMyDataFileHeaderAccess = CreateDataFileHeaderAccess
oMyDataStore            = oMyDataFileHeaderAccess.Open(dd.DataReadPath + "Example.tdm" ,"TDM", False)
print(oMyDataStore.RootElements(1).Children(1).Children(2).Name)
```

```python
oMyDataFileHeaderAccess = CreateDataFileHeaderAccess
oMyFolder = dd.ProgramDrv + "Examples\\Data\\"
# Open TDM file to change header
oMyDataStore = oMyDataFileHeaderAccess.Open(oMyFolder + "Example_data.tdm" ,"TDM", False)

#---  Change custom root properties -------------------------
oRoot = oMyDataStore.RootElements(1)
oRootPropColl = oRoot.Properties

oRootPropColl.ListInstanceProperties = True
if oRootPropColl.Exists("CustomRootProp") :
    oRootCustomProp = oRootPropColl("CustomRootProp")
else:
    oRootCustomProp = oRootPropColl.Add("CustomRootProp","RootValue",dd.eString)
print(oRootPropColl("CustomRootProp").Value)

#--- Change custom group properties -------------------------
oGroup       = oRoot.Children(3)
oGroupPropColl = oGroup.Properties

oGroupPropColl.ListInstanceProperties = True
if oGroupPropColl.Exists("CustomGroupProp") :
    oGroupCustomProp = oGroupPropColl("CustomGroupProp")
else:
    oGroupCustomProp = oGroupPropColl.Add("CustomGroupProp","GroupValue",dd.eString)
print (oGroupPropColl("CustomGroupProp").Value)

#---  Change custom channel properties ------------------------
oChannel   = oGroup.Children(4)
oChnPropColl = oChannel.Properties

oChnPropColl.ListInstanceProperties = True
if oChnPropColl.Exists("CustomChannelProp") :
    oChannelCustomProp = oChnPropColl("CustomChannelProp")
else:
    oChannelCustomProp = oChnPropColl.Add("CustomChannelProp","ChannelValue",dd.eString)
print (oChnPropColl("CustomChannelProp").Value)

# Save file
oMyDataStore.Save()
```

## See also

<div markdown="1">
<div class="SeeAlso">
</div>
</div>

---

*Source: `ComOff/TDM_Method_CreateDataFileHeaderAccess.htm`*
