---
title: "IDiademProperty.Value"
description: "Specifies the value of a property in the script interface for internal data."
---

# IDiademProperty.Value

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Value for Property <Data>

Specifies the value of a property in the script interface for internal data.

## Signature

```python
obj.Value
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong> In VBS scripts you can use the Navigator-API to assign time values to a DIAdem time property as a <a href="../../../scriptnavi/properties/itdmtimedisp-variantdate/">VariantDate</a> object or as a <a href="../../../scriptnavi/objects/itdmtimedisp/">UsiTimeDisp</a> object. <span class="style1">Use the <a href="../../../scriptnavi/objects/itdmtimedisp/">UsiTimeDisp</a>object if you have enabled the <a href="../../../varoff/variables/applicationtimebasehighresolution/">High resolution for absolute time values</a> setting under <strong>Settings»DIAdem Settings»General</strong>. Use the <a href="../../../comoff/commands/createtime/">CreateTime</a> command or the <strong>oValue</strong> property to create a high-resolution time object of type <a href="../../../scriptnavi/objects/itdmtimedisp/">UsiTimeDisp</a>.</span><p>When working with date/time values, pay attention to the following characteristics:</p><ul><li>The <strong>Value</strong> property returns a <span class="Monospace">VBDate</span> data type value. This data type has a valid range from 01/01/100 to 31/12/9999 23:59:59. On 30/12/1899 you can only use time information but no date information. If you convert <span class="Monospace">VBDate</span> type values that contain only time information into the USITimeDisp format, the program automatically adds the 01/01/0000 date information. The <span class="Monospace">VBDate</span> type <span class="Monospace">Value</span> property contains a maximum of 4 decimal places.  If you convert <span class="Monospace">VBDate</span> type values into the DIAdem time format, the program adds the date information in relation to the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a>.</li>
<li>Use the <strong>oValue</strong> property instead of the <strong>Value</strong>property if you are working with time values that lie within the range between January 1 of year zero and 01/01/100, or concern December 30, 1899. The <strong>oValue</strong> property returns time values as <a href="../../../scriptnavi/objects/itdmtimedisp/">USITimeDisp object</a> in the USITimeDisp format. The USITimeDisp object is valid from 01/01 of the year zero to 12/31/9999 23:59:59.</li>
<li>You cannot assign <span class="Monospace">NoValue</span> to date/time type properties. You can only assign <span class="Monospace">NoValue</span> to channel values that are double types.</li></ul></td></tr></table>
</div>

## Python example

```python
for prop in dd.Data.Root.Properties:
    print(prop.Name, prop.Value, sep=": ")
```

```python
if dd.Navigator.Display.CurrDataFinder.Browser.FocusedElement.IsKindOf(dd.eSearchFile):
    file_date = dd.Navigator.Display.CurrDataFinder.Browser.FocusedElement.Properties("DateTime").Value
    dd.Data.Root.Properties("DateTime").Value = file_date
    print(dd.Data.Root.Properties("DateTime").Value)
else:
    print("Please select a file in the browser.")
```

```python
# No Python script example available.
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Value_IDiademProperty.HTM`*
