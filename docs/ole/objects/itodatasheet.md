---
title: "ITODataSheet"
description: "The interface TODataSheet facilitates access to the DIAdem data area. Always use the bInterfaceLocked property to request the status of the DIAdem OLE interface"
---

# ITODataSheet

!!! abstract "Object &middot; `OLE.chm`"
    Object: TODataSheet

The interface TODataSheet facilitates access to the DIAdem data area. Always use the bInterfaceLocked property to request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an OLE command to DIAdem although the property has the value True , the behavior of DIAdem is unpredictable.

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
while True:
    if not oDIAdem.bInterfaceLocked:
            break
iSuccess = oDIAdem.ChnCommentGet(5, vCommentP)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itodatasheet-binterfacelocked/">bInterfaceLocked</a> | <a href="../../properties/itodatasheet-bnoactivitydisplay/">bNoActivityDisplay</a> | <a href="../../properties/itodatasheet-bnodialogdisplay/">bNoDialogDisplay</a> | <a href="../../properties/itodatasheet-bnoerrordisplay/">bNoErrorDisplay</a> | <a href="../../properties/itodatasheet-bnoinfodisplay/">bNoInfoDisplay</a> | <a href="../../properties/itodatasheet-bnomsgdisplay/">bNoMsgDisplay</a> | <a href="../../properties/itodatasheet-bnowarningdisplay/">bNoWarningDisplay</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itodatasheet-chncommentget/">ChnCommentGet</a> | <a href="../../methods/itodatasheet-chncommentset/">ChnCommentSet</a> | <a href="../../methods/itodatasheet-chndatatypeget/">ChnDataTypeGet</a> | <a href="../../methods/itodatasheet-chndatatypeset/">ChnDataTypeSet</a> | <a href="../../methods/itodatasheet-chndimget/">ChnDimGet</a> | <a href="../../methods/itodatasheet-chndimset/">ChnDimSet</a> | <a href="../../methods/itodatasheet-chnlengthget/">ChnLengthGet</a> | <a href="../../methods/itodatasheet-chnlengthset/">ChnLengthSet</a> | <a href="../../methods/itodatasheet-chnnameget/">ChnNameGet</a> | <a href="../../methods/itodatasheet-chnnameset/">ChnNameSet</a> | <a href="../../methods/itodatasheet-chnparamsupdate/">ChnParamsUpdate</a> | <a href="../../methods/itodatasheet-chnvalget/">ChnValGet</a> | <a href="../../methods/itodatasheet-chnvalset/">ChnValSet</a> | <a href="../../methods/itodatasheet-maxchncountget/">MaxChnCountGet</a> | <a href="../../methods/itodatasheet-maxchnlengthget/">MaxChnLengthGet</a> | <a href="../../methods/itodatasheet-updateparamslock/">UpdateParamsLock</a> | <a href="../../methods/itodatasheet-valuerangeformatedget/">ValueRangeFormatedGet</a> | <a href="../../methods/itodatasheet-valuerangeformatedset/">ValueRangeFormatedSet</a> | <a href="../../methods/itodatasheet-valuerangeget/">ValueRangeGet</a> | <a href="../../methods/itodatasheet-valuerangeset/">ValueRangeSet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/objects/OLE_Objects_ITODataSheet.htm`*
