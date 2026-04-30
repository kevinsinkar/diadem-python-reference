---
title: "IDocumentProperty.DataType"
description: "Returns the data type of a meta property of a document. Use the method Add for DocumentProperties <Data> to create new meta properties. A document may be an Off"
---

# IDocumentProperty.DataType

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: DataType for DocumentProperty <Data>

Returns the data type of a meta property of a document. Use the method Add for DocumentProperties <Data> to create new meta properties. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.DataType
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
for oMyProperty in oMyDocument.Properties:
    sOut = sOut + "Name: " + oMyProperty.Name + ", Data type: " + PropertyDataTypeAsText(oMyProperty.DataType) + "\r\n"
print(sOut)

# Function to convert data type from integer into text ===
def PropertyDataTypeAsText(eMyType):
    select_variable_0 = eMyType
    if (select_variable_0 == dd.DataTypeDocumentInt32) :
        PropertyDataTypeAsText = "Int32"
    elif (select_variable_0 == dd.DataTypeDocumentFloat64) :
        PropertyDataTypeAsText = "Float64"
    elif (select_variable_0 == dd.DataTypeDocumentString) :
        PropertyDataTypeAsText = "String"
    elif (select_variable_0 == dd.DataTypeDocumentDate) :
        PropertyDataTypeAsText = "Date"
    return PropertyDataTypeAsText
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/properties/DiaCmpnt_property_DataType_IDocumentProperty.htm`*
