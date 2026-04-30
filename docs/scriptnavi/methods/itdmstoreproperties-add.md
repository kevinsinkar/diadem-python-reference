---
title: "ITDMStoreProperties.Add"
description: "Generates in a data store a new instance property with a value. To generate an instance property, the ListInstanceProperties property must have the value TRUE."
---

# ITDMStoreProperties.Add

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Add for Properties <DataStore>

Generates in a data store a new instance property with a value. To generate an instance property, the ListInstanceProperties property must have the value TRUE.

## Signature

```python
return_value = obj.Add(Name, Value, Type)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You must not use any of the following characters in a property name: <span class="Monospace">.</span>, <span class="Monospace">:</span>, <span class="Monospace">,</span>, <span class="Monospace">;</span>, <span class="Monospace">'</span>, <span class="Monospace">\</span>, <span class="Monospace">@</span>, <span class="Monospace">&lt;</span>, <span class="Monospace">&gt;</span>, <span class="Monospace">#</span>, <span class="Monospace">[</span>, <span class="Monospace">]</span>, <span class="Monospace">%</span>, <span class="Monospace">(</span>, <span class="Monospace">)</span>, <span class="Monospace">{</span>, <span class="Monospace">}</span>, <span class="Monospace">|</span>, <span class="Monospace">*</span>, <span class="Monospace">?</span>, <span class="Monospace">=</span>, <span class="Monospace">!</span>, <span class="Monospace">"</span>, <span class="Monospace">^</span>, <span class="Monospace">$</span>, <span class="Monospace">&amp;</span>, <span class="Monospace">+</span>, <span class="Monospace">-</span>, <span class="Monospace">/</span>, and a space. The name of a property must start with a letter from the alphabet (a-z, A-Z).</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Enumeration` | 24 | DataTypeEnum |

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyProperties = oMyDataStore.RootElements(1).Properties
oMyProperties.ListInstanceProperties = True
oMyProperties.Add("MyProperty", "MyText", 23)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Add_ITDMStoreProperties.htm`*
