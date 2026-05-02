---
title: "IDataFileHeader"
description: "The DataFileHeader object provides methods, which you can use to read, write, modify, or delete channel properties, group properties, or file properties from TD"
---

# IDataFileHeader

!!! abstract "Object &middot; `TDMScript.chm`"
    Object: DataFileHeader

The DataFileHeader object provides methods, which you can use to read, write, modify, or delete channel properties, group properties, or file properties from TDM files or TDMS files. You also can use this object to read headers from DataPlugins. Use the DataFileHeaderAccess method to create a DataFileHeader object.

## Python example

```python
oMyDataFileHeader = dd.CreateDataFileHeaderAccess(dd.DataLibrPath + "Example.tdm","TDM",False)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatafileheader-filename/">FileName</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatafileheader-chnnameget/">ChnNameGet</a> | <a href="../../methods/idatafileheader-chnpropcount/">ChnPropCount</a> | <a href="../../methods/idatafileheader-chnpropdatatypeget/">ChnPropDataTypeGet</a> | <a href="../../methods/idatafileheader-chnpropdel/">ChnPropDel</a> | <a href="../../methods/idatafileheader-chnpropexist/">ChnPropExist</a> | <a href="../../methods/idatafileheader-chnpropisfixed/">ChnPropIsFixed</a> | <a href="../../methods/idatafileheader-chnpropnameget/">ChnPropNameGet</a> | <a href="../../methods/idatafileheader-chnpropvalget/">ChnPropValGet</a> | <a href="../../methods/idatafileheader-chnpropvalset/">ChnPropValSet</a> | <a href="../../methods/idatafileheader-close/">Close</a> | <a href="../../methods/idatafileheader-groupchncount/">GroupChnCount</a> | <a href="../../methods/idatafileheader-groupchnmove/">GroupChnMove</a> | <a href="../../methods/idatafileheader-groupchnswap/">GroupChnSwap</a> | <a href="../../methods/idatafileheader-groupcount/">GroupCount</a> | <a href="../../methods/idatafileheader-groupmove/">GroupMove</a> | <a href="../../methods/idatafileheader-groupnameget/">GroupNameGet</a> | <a href="../../methods/idatafileheader-grouppropcount/">GroupPropCount</a> | <a href="../../methods/idatafileheader-grouppropdatatypeget/">GroupPropDataTypeGet</a> | <a href="../../methods/idatafileheader-grouppropdel/">GroupPropDel</a> | <a href="../../methods/idatafileheader-grouppropexist/">GroupPropExist</a> | <a href="../../methods/idatafileheader-grouppropisfixed/">GroupPropIsFixed</a> | <a href="../../methods/idatafileheader-grouppropnameget/">GroupPropNameGet</a> | <a href="../../methods/idatafileheader-grouppropvalget/">GroupPropValGet</a> | <a href="../../methods/idatafileheader-grouppropvalset/">GroupPropValSet</a> | <a href="../../methods/idatafileheader-groupswap/">GroupSwap</a> | <a href="../../methods/idatafileheader-rootpropcount/">RootPropCount</a> | <a href="../../methods/idatafileheader-rootpropdatatypeget/">RootPropDataTypeGet</a> | <a href="../../methods/idatafileheader-rootpropdel/">RootPropDel</a> | <a href="../../methods/idatafileheader-rootpropexist/">RootPropExist</a> | <a href="../../methods/idatafileheader-rootpropisfixed/">RootPropIsFixed</a> | <a href="../../methods/idatafileheader-rootpropnameget/">RootPropNameGet</a> | <a href="../../methods/idatafileheader-rootpropvalget/">RootPropValGet</a> | <a href="../../methods/idatafileheader-rootpropvalset/">RootPropValSet</a> | <a href="../../methods/idatafileheader-save/">Save</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p></div>
</div>

---

*Source: `TDMScript/objects/TDM_Objects_IDataFileHeader.htm`*
