---
title: "Methods (INaviData (Data Model Interfaces))"
---

# Methods

105 methods from `Inavidata.chm`.

| Name | Summary |
| --- | --- |
| [`IAssignmentList.Add`](iassignmentlist-add.md) | Creates a new assignment in the assignment list of an assignment channel in the script interface for internal data . |
| [`IAssignmentList.Exists`](iassignmentlist-exists.md) | Checks in the script interface for internal data whether an assignment with the specified text value already exists in an assignment channel. |
| [`IAssignmentList.ExistsByDefinition`](iassignmentlist-existsbydefinition.md) | Checks in the script interface for internal data whether the assignment with a specified definition value already exists in an assignment channel. |
| [`IAssignmentList.FindByDefinition`](iassignmentlist-findbydefinition.md) | Uses the value to determine an assignment of texts to values in the script interface for internal data. |
| [`IAssignmentList.FindByValue`](iassignmentlist-findbyvalue.md) | Uses the text to determine an assignment of texts to values in the script interface for internal data. |
| [`IAssignmentList.Item`](iassignmentlist-item.md) | Returns the assignment of a specified index in the script interface for internal data. |
| [`IAssignmentList.Remove`](iassignmentlist-remove.md) | Deletes an assignment from the assignment list of an assignment channel in the script interface for internal data. |
| [`IAssignmentList.RemoveAll`](iassignmentlist-removeall.md) | Deletes all assignments of an assignment channel in the script interface for internal data. |
| [`IAssignmentList.SetBoundaryLimits`](iassignmentlist-setboundarylimits.md) | Specifies the behavior at the interval limits of the minimum and maximum values of an assignment, in the script interface for internal data. |
| [`IDataTemplate.Clear`](idatatemplate-clear.md) | Deletes all custom properties from the custom properties template in the script interface for internal data. |
| [`IDiademAbstractChannel.GetReference`](idiademabstractchannel-getreference.md) | Returns a channel reference of a channel in the script interface for internal data. |
| [`IDiademAbstractChannel.GetValuesBlock`](idiademabstractchannel-getvaluesblock.md) | Reads out a block of values from a channel in the Data Portal and writes these values into an array. |
| [`IDiademAbstractChannel.IsKindOf`](idiademabstractchannel-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDiademAbstractChannel.RemoveValues`](idiademabstractchannel-removevalues.md) | Deletes the specified values from a channel. DIAdem moves up the subsequent values. |
| [`IDiademAbstractChannel.XRelation`](idiademabstractchannel-xrelation.md) | Specifies the x-channel for an xy-channel . The x-channel must be in the same channel group as the y-channels. You cannot convert waveform channels into xy-channels because waveform channels already contain the x-part. |
| [`IDiademAssignmentChannel.GetReference`](idiademassignmentchannel-getreference.md) | Returns the channel reference of an assignment channel, in the script interface for internal data. Use this method when you are working with data objects and need channel references for calculations or for layout configurations. |
| [`IDiademAssignmentChannel.GetValuesBlock`](idiademassignmentchannel-getvaluesblock.md) | Reads out a block of values from an assignment channel in the Data Portal and writes these values into an array. |
| [`IDiademAssignmentChannel.IsKindOf`](idiademassignmentchannel-iskindof.md) | Checks the type of an assignment channel in the script interface for internal data. |
| [`IDiademAssignmentChannel.RemoveValues`](idiademassignmentchannel-removevalues.md) | Deletes the specified values from an assignment channel. DIAdem moves up the subsequent values. |
| [`IDiademAssignmentChannel.SetValues`](idiademassignmentchannel-setvalues.md) | Inserts a numeric value n times at the specified position into an assignment channel. |
| [`IDiademAssignmentChannel.SetValuesBlock`](idiademassignmentchannel-setvaluesblock.md) | Inserts a block of numeric values from an array into an assignment channel in the Data Portal. |
| [`IDiademAssignmentChannel.XRelation`](idiademassignmentchannel-xrelation.md) | Specifies the x-channel for an xy-channel . The x-channel must be in the same channel group as the y-channels. You cannot convert waveform channels into xy-channels because waveform channels already contain the x-part. |
| [`IDiademCalculationChannel.GetReference`](idiademcalculationchannel-getreference.md) | Determines a reference to a calculation of the calculation manager in the script interface for internal data. |
| [`IDiademCalculationChannel.GetValuesBlock`](idiademcalculationchannel-getvaluesblock.md) | Reads a block of values from a calculation channel in the Data Portal and writes these values into an array. |
| [`IDiademCalculationChannel.IsKindOf`](idiademcalculationchannel-iskindof.md) | Checks the type of a calculation channel in the script interface for internal data. If the IsKindOf method for eDataCalculationChannelFormula returns the value True, you can access the Formula property. If the IsKindOf method for eDataCalculationChannelReference returns the value True, you can access the Formula property. |
| [`IDiademCalculationChannel.RunCalculation`](idiademcalculationchannel-runcalculation.md) | Runs a calculation in the script interface for internal data to determine the values of a calculation channel. When you create a calculation channel, DIAdem calculates the channel values automatically; you do not need to call the RunCalculation method. If the values of the channels in the calculation change, DIAdem updates the channel values when you restart the calculation using the RunCalculation method. If DIAdem cannot calculate the values of a calculation channel because, for example, an input channel is missing, DIAdem deletes all values and the unit of the calculation channel as soon as you update the values of this channel. |
| [`IDiademCalculationChannel.XRelation`](idiademcalculationchannel-xrelation.md) | Specifies the x-channel for an xy-channel in the script interface for internal data. The x-channel must be in the same channel group as the y-channel. |
| [`IDiademChannel.GetReference`](idiademchannel-getreference.md) | Returns a channel reference of a channel in the script interface for internal data. Use this method when you are working with data objects and need channel references for calculations or for layout configurations. |
| [`IDiademChannel.GetValuesBlock`](idiademchannel-getvaluesblock.md) | Reads out a block of values from a channel in the Data Portal and writes these values into an array. |
| [`IDiademChannel.IsKindOf`](idiademchannel-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDiademChannel.RemoveValues`](idiademchannel-removevalues.md) | Deletes the specified values from a channel. DIAdem moves up the subsequent values. |
| [`IDiademChannel.SetValues`](idiademchannel-setvalues.md) | Inserts the value n times at the specified position into a channel. |
| [`IDiademChannel.SetValuesBlock`](idiademchannel-setvaluesblock.md) | Inserts a block of values from an array into a channel in the Data Portal. |
| [`IDiademChannel.XRelation`](idiademchannel-xrelation.md) | Specifies the x-channel for an xy-channel . The x-channel must be in the same channel group as the y-channels. You cannot convert waveform channels into xy-channels because waveform channels already contain the x-part. |
| [`IDiademChannelGroup.Activate`](idiademchannelgroup-activate.md) | Specifies a channel group as the default group in the script interface for internal data. |
| [`IDiademChannelGroup.IsKindOf`](idiademchannelgroup-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDiademChannelGroups.Add`](idiademchannelgroups-add.md) | Creates a new channel group in the script interface for internal data and adds the channel group to the ChannelGroups collection. The Add method returns a ChannelGroup object. |
| [`IDiademChannelGroups.AddChannelGroup`](idiademchannelgroups-addchannelgroup.md) | Copies a ChannelGroup object in the script interface for internal data and adds the object to the existing ChannelGroup objects. |
| [`IDiademChannelGroups.Exists`](idiademchannelgroups-exists.md) | Checks whether a ChannelGroup object with a specific name already exists in the channel groups collection in the script interface for internal data. |
| [`IDiademChannelGroups.item`](idiademchannelgroups-item.md) | Returns the ChannelGroup object of a specific name or of a specific index in the script interface for internal data. |
| [`IDiademChannelGroups.Remove`](idiademchannelgroups-remove.md) | Deletes one element from the ChannelGroups collection in the script interface for internal data. |
| [`IDiademChannelGroups.RemoveAll`](idiademchannelgroups-removeall.md) | Deletes all elements from the ChannelGroups collection in the script interface for internal data. |
| [`IDiademChannelGroups.Sort`](idiademchannelgroups-sort.md) | Sorts the channel groups in the Data Portal alphabetically in the script interface for internal data. |
| [`IDiademChannels.Add`](idiademchannels-add.md) | Creates a new channel in the script interface for internal data and adds the channel to the Channels collection. The Add method returns a Channel object. |
| [`IDiademChannels.AddAssignmentChannel`](idiademchannels-addassignmentchannel.md) | Creates a new assignment channel in the script interface for internal data. |
| [`IDiademChannels.AddCalculationChannel`](idiademchannels-addcalculationchannel.md) | Generates, in the script interface for internal data, a new calculation channel in the current channel group with a simple single-line formula. |
| [`IDiademChannels.AddCalculationChannelRef`](idiademchannels-addcalculationchannelref.md) | Generates a new calculation channel with a reference to a calculation of the calculation manager in the script interface for internal data. Use the AddCalculationChannel method to create a new calculation channel using a simple one-line formula. |
| [`IDiademChannels.AddChannel`](idiademchannels-addchannel.md) | Copies an existing channel in a collection of other channels in the script interface for internal data. |
| [`IDiademChannels.AddImplicitChannel`](idiademchannels-addimplicitchannel.md) | Creates a new implicit channel in the script interface for internal data. |
| [`IDiademChannels.AddVideoChannel`](idiademchannels-addvideochannel.md) | Generates a new video channel in the script interface for internal data. |
| [`IDiademChannels.Exists`](idiademchannels-exists.md) | Checks whether a Channel object with a specific name already exists in the Channels <Data> collection in the script interface for internal data. The Channels <Data> collection contains all channels of a channel group. |
| [`IDiademChannels.GetReference`](idiademchannels-getreference.md) | Returns the channel reference of channels in a list, in the script interface for internal data. Use this method when you are working with data objects and need channel references for calculations or for layout configurations. |
| [`IDiademChannels.item`](idiademchannels-item.md) | Returns the Channel object of a specific name or of a specific index in the script interface for internal data. |
| [`IDiademChannels.Remove`](idiademchannels-remove.md) | Deletes one element from the Channels collection in the script interface for internal data. |
| [`IDiademChannels.RemoveAll`](idiademchannels-removeall.md) | Deletes all elements from the Channels collection in the script interface for internal data. |
| [`IDiademChannels.Sort`](idiademchannels-sort.md) | Sorts the channels of a channel group in the Data Portal alphabetically in the script interface for internal data. |
| [`IDiademComplexChannel.GetReference`](idiademcomplexchannel-getreference.md) | Returns the channel reference of a complex channel in the script interface for internal data. Use this method when you are working with data objects and need channel references for calculations or for layout configurations. |
| [`IDiademComplexChannel.GetValuesBlock`](idiademcomplexchannel-getvaluesblock.md) | Reads a block of values from a complex channel in the Data Portal and writes these values into an array. |
| [`IDiademComplexChannel.IsKindOf`](idiademcomplexchannel-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDiademComplexChannel.RemoveValues`](idiademcomplexchannel-removevalues.md) | Deletes the specified values from a complex channel . DIAdem moves up the subsequent values. |
| [`IDiademComplexChannel.SetValues`](idiademcomplexchannel-setvalues.md) | Inserts the value n times at the specified position into a complex channel . |
| [`IDiademComplexChannel.SetValuesBlock`](idiademcomplexchannel-setvaluesblock.md) | Inserts a block of values from an array into a complex channel in the Data Portal. |
| [`IDiademComplexChannel.XRelation`](idiademcomplexchannel-xrelation.md) | Specifies the x-channel for a complex xy-channel . The x-channel must be in the same channel group as the y-channels. You cannot convert waveform channels into xy-channels because waveform channels already contain the x-part. |
| [`IDiademElementList.Add`](idiademelementlist-add.md) | Creates a new element in the script interface for internal data and adds this element to the ElementList collection. The Add method returns an Element object. This method is not available if the ElementList collection is read-only. |
| [`IDiademElementList.AddElementList`](idiademelementlist-addelementlist.md) | Connects two element lists in the Script interface for internal data. |
| [`IDiademElementList.Exists`](idiademelementlist-exists.md) | Checks in the script interface for internal data whether a data element already exists. The Exists method checks when the data element first occurs in the elements list. |
| [`IDiademElementList.Item`](idiademelementlist-item.md) | Returns the ElementList object of a specific index in the script interface for internal data. |
| [`IDiademElementList.Remove`](idiademelementlist-remove.md) | Deletes one element from the ElementList collection in the script interface for internal data. This method is not available if the ElementList collection is read-only. |
| [`IDiademElementList.RemoveAll`](idiademelementlist-removeall.md) | Deletes all elements from the ElementList collection in the script interface for internal data. This method is not available if the ElementList collection is read-only. |
| [`IDiademImplicitChannel.GetReference`](idiademimplicitchannel-getreference.md) | Returns the channel reference of an implicit channel in the script interface for internal data. |
| [`IDiademImplicitChannel.GetValuesBlock`](idiademimplicitchannel-getvaluesblock.md) | Reads out a block of values from an implicit channel in the Data Portal and writes these values into an array. |
| [`IDiademImplicitChannel.IsKindOf`](idiademimplicitchannel-iskindof.md) | Checks the type of an implicit channel in the script interface for internal data. |
| [`IDiademImplicitChannel.XRelation`](idiademimplicitchannel-xrelation.md) | Specifies the x-channel for an xy-channel . The x-channel must be in the same channel group as the y-channels. You cannot convert waveform channels into xy-channels because waveform channels already contain the x-part. |
| [`IDiademProperties.Add`](idiademproperties-add.md) | Generates a new property with a value in the script interface for internal data. If the property already exists, DIAdem changes only the value of the property. If the property does not exist, DIAdem generates a new custom property. The Add method returns a Property object. |
| [`IDiademProperties.AddProperties`](idiademproperties-addproperties.md) | Adds copies of existing properties to the properties of an element (root, channel group, or channel), in the script interface for internal data. |
| [`IDiademProperties.Exists`](idiademproperties-exists.md) | Checks whether a Property object with a specific name already exists in the properties collection in the script interface for internal data. |
| [`IDiademProperties.item`](idiademproperties-item.md) | Returns the Property object of a specific name or of a specific index in the script interface for internal data. |
| [`IDiademProperties.Remove`](idiademproperties-remove.md) | Deletes a custom property from the Properties collection in the script interface for internal data. |
| [`IDiademProperties.RemoveAll`](idiademproperties-removeall.md) | Deletes all custom properties from the Properties collection in the script interface for internal data. |
| [`IDiademPropertyList.Add`](idiadempropertylist-add.md) | Creates a new element in the script interface for internal data and adds this element to the PropertyList collection. The Add method returns an Element object. This method is not available if the PropertyList collection is read-only. |
| [`IDiademPropertyList.AddPropertyList`](idiadempropertylist-addpropertylist.md) | Copies a list of properties to the end of a different list of properties in the script interface for internal data. |
| [`IDiademPropertyList.Item`](idiadempropertylist-item.md) | Returns a single property of the Root object, the ChannelGroup object, or the Channel object which belongs to a specified index. |
| [`IDiademPropertyList.Remove`](idiadempropertylist-remove.md) | Deletes one element from the PropertyList collection in the script interface for internal data. This method is not available if the PropertyList collection is read-only. |
| [`IDiademPropertyList.RemoveAll`](idiadempropertylist-removeall.md) | Deletes all elements from the PropertyList collection in the script interface for internal data. This method is not available if the PropertyList collection is read-only. |
| [`IDiademRoot.Clear`](idiademroot-clear.md) | Deletes all the internal DIAdem data in the script interface for internal data. |
| [`IDiademRoot.IsKindOf`](idiademroot-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDiademUSIElement.IsKindOf`](idiademusielement-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDiademVideoChannel.GetReference`](idiademvideochannel-getreference.md) | Returns a channel reference of a channel in the script interface for internal data. Use this method when you are working with data objects and need channel references for calculations or for layout configurations. |
| [`IDiademVideoChannel.IsKindOf`](idiademvideochannel-iskindof.md) | Checks the type of an element in the script interface for internal data. |
| [`IDropInformation.IsKindOf`](idropinformation-iskindof.md) | Checks whether a DropInformation object is a certain type. |
| [`IFileList.Add`](ifilelist-add.md) | Adds an element to a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list. |
| [`IFileList.Item`](ifilelist-item.md) | Returns in a file list that you drag and drop to another object the file or folder associated with a specific index. |
| [`IFileList.Remove`](ifilelist-remove.md) | Deletes an element in a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list. |
| [`IFileList.RemoveAll`](ifilelist-removeall.md) | Deletes all elements of a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list. |
| [`INaviData.CreateElementList`](inavidata-createelementlist.md) | Generates in the script interface for internal data a collection of elements. Every element from the generated collection is an Element and thus can be a root type (eDataRoot), a channel group type (eDataChannelgroup), or a channel type (eDataChannel). |
| [`INaviData.GetChannel`](inavidata-getchannel.md) | Returns a channel in the script interface for internal data. |
| [`INaviData.GetChannelGroups`](inavidata-getchannelgroups.md) | Returns a collection of channel groups in the script interface for internal data. |
| [`INaviData.GetChannels`](inavidata-getchannels.md) | Returns a collection of channels in the script interface for internal data. DIAdem sorts the result list in ascending channel number order. Use the GetChannels method to create data objects from channel references, for example, from layout configurations, and then to continue processing the data using the script interface for internal data. |
| [`INaviData.Move`](inavidata-move.md) | Moves in the script interface for internal data a channel group or a channel to a different position in the Data Portal. |
| [`INaviData.Remove`](inavidata-remove.md) | Deletes a list of elements from the Data Portal, in the script interface for internal data. |
| [`ITemplateProperties.Add`](itemplateproperties-add.md) | Generates a new custom properties template with a value in the script interface for internal data. If the custom properties template already exists, DIAdem changes only the value of this custom properties template. If the custom properties template does not exist, DIAdem creates a new custom properties template. The Add method returns a TemplateProperty object. |
| [`ITemplateProperties.Exists`](itemplateproperties-exists.md) | Checks whether a TemplateProperty object with a specific name already exists in the collection of custom properties templates in the script interface for internal data. |
| [`ITemplateProperties.Item`](itemplateproperties-item.md) | Returns the TemplateProperty object that is associated with a specific name or a specific index, in the script interface for internal data. |
| [`ITemplateProperties.Remove`](itemplateproperties-remove.md) | Deletes a custom property from the TemplateProperties collection in the script interface for internal data. |
| [`ITemplateProperties.RemoveAll`](itemplateproperties-removeall.md) | Deletes all custom properties from the TemplateProperties collection in the script interface for internal data. |
