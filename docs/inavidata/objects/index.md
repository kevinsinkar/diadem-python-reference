---
title: "Objects (INaviData (Data Model Interfaces))"
---

# Objects

17 objects from `Inavidata.chm`.

| Name | Summary |
| --- | --- |
| [`IAssignment`](iassignment.md) | The assignment object provides an individual assignment of an assignment channel in the script interface for internal data. A text value (property Value ) is assigned to a numeric value (property Definition ) or to a value range (property DefinitionRange ) in order to define an assignment. |
| [`IDataSettings`](idatasettings.md) | The Settings object provides access to the general DIAdem settings in the script interface for internal data. |
| [`IDataTemplate`](idatatemplate.md) | The CustomPropertyTemplate object provides a custom properties template in the script interface for internal data. |
| [`IDiademAbstractChannel`](idiademabstractchannel.md) | The BaseChannel object provides a channel and the associated Properties in the script interface for internal data. The BaseChannel object corresponds to one of the following objects: AssignmentChannel (IDiademAssignmentChannel) Assignment channel CalculationChannel (IDiademCalculationChannel) Calculation Channel Channel (IDiademChannel) Numeric or text channel ImplicitChannel (IDiademImplicitChannel) Implicit channel |
| [`IDiademAssignmentChannel`](idiademassignmentchannel.md) | The AssignmentChannel object provides an assignment channel in the script interface for internal data. |
| [`IDiademCalculationChannel`](idiademcalculationchannel.md) | The CalculationChannel <Data> object provides a calculation channel . Use the AddCalculationChannel method to create a new calculation channel using a simple single-line formula and the AddCalculationChannelRef method to create a new calculation channel with a reference to a calculation of the calculation manager. |
| [`IDiademChannel`](idiademchannel.md) | The Channel object provides a channel and the associated Properties in the script interface for internal data. The Channel object is an element of the Channels collection. |
| [`IDiademChannelGroup`](idiademchannelgroup.md) | The ChannelGroup object provides a channel group and the associated channels and Properties in the script interface for internal data. The ChannelGroup object is an element of the ChannelGroups collection. |
| [`IDiademComplexChannel`](idiademcomplexchannel.md) | ComplexChannel <Data> object provides a complex channel in the script interface for internal data. The Channel object is an element of the Channels collection. Complex channels are a preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change. |
| [`IDiademImplicitChannel`](idiademimplicitchannel.md) | The ImplicitChannel object provides an implicit channel in the interface for internal data. An implicit channel contains linear generation specifications, which describes the data, instead of single values. |
| [`IDiademProperty`](idiademproperty.md) | The Property object provides a property for the Root object, for the ChannelGroup object, or for the Channel object in the script interface for internal data. This property is either a DIAdem base property or a custom property. The Property object is an element of the Properties or PropertyList collection. |
| [`IDiademRoot`](idiademroot.md) | The Root object provides the collection of all the channel groups and all the Properties of the data set in the script interface for internal data. |
| [`IDiademUSIElement`](idiademusielement.md) | The Element object provides a single element in the script interface for internal data. Depending on whether an element of the internal data is a data set ( Root ), a group ( ChannelGroup ), or a channel ( Channel ), the Element object has additional properties. Use the IsKindOf method to determine the type of an element. Refer to Working with the Elements Collection and the Element Object for general information on working with the elements. |
| [`IDiademVideoChannel`](idiademvideochannel.md) | The VideoChannel <Data> object provides a video channel . |
| [`IDropInformation`](idropinformation.md) | The DropInformation object provides information about the object which you drag and drop onto another object. In DIAdem you can, for example, drag elements such as groups, channels, properties, text, or files from the explorer onto another element. As a target you can use, for example, a worksheet or objects in DIAdem REPORT, areas in DIAdem VIEW, or parts of a user dialog box. |
| [`INaviData`](inavidata.md) | The Data object accesses the internal DIAdem data. You use the Data object to generate, to edit, and to delete channel groups and channels with the associated properties. The Data object is available as a global object in scripts and in dialog boxes. Only read access. |
| [`ITemplateProperty`](itemplateproperty.md) | The Property object provides a custom properties template of the data set ( Root ), of a Channel group , or of a Channel in the script interface for internal data. The TemplateProperty object is an element of the TemplateProperties collection. |
