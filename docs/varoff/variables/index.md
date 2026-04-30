---
title: "Variables (Global Script Variables (Offline))"
---

# Variables

3211 variables from `VarOff.chm`.

| Name | Summary |
| --- | --- |
| [`ACDCWndFct`](acdcwndfct.md) | Specifies which window function DIAdem uses on the entire input channel. |
| [`ACompAverage`](acompaverage.md) | Receives the average acceleration of the AComp calculation. |
| [`ACompEndTime`](acompendtime.md) | Receives the end time for the AComp calculation. |
| [`ACompSpeed0`](acompspeed0.md) | Specifies the start value of the velocity in the AComp calculation. |
| [`ACompSpeedFactor`](acompspeedfactor.md) | Specifies the factor for the conversion of the units in the AComp calculation. |
| [`ACompStartTime`](acompstarttime.md) | Specifies the start time for the AComp calculation. |
| [`ACompTangentType`](acomptangenttype.md) | Specifies the tangent type for the AComp calculation. |
| [`ACompVer`](acompver.md) | Valid names: ACompVer, ACompVersion |
| [`ActArrayDrv`](actarraydrv.md) | Specifies the path for swapping out the data area. |
| [`ActFileHdNo`](actfilehdno.md) | Specifies the maximum number of channels that DIAdem can read from a DAT file and can edit. |
| [`ActWPageArea`](actwpagearea.md) |  |
| [`ActXPage`](actxpage.md) |  |
| [`ActYPage`](actypage.md) |  |
| [`AddOnParaFile`](addonparafile.md) |  |
| [`ADOConString`](adoconstring.md) | Receives the ADO connection string. |
| [`AkimaCoeff`](akimacoeff.md) | Specifies the influence of the neighboring interpolation points when DIAdem approximates the interpolation points, for Akima subsplines. |
| [`AkimaFit`](akimafit.md) | Specifies whether DIAdem uses an interpolating or an approximating curve type for Akima subsplines. |
| [`AkimaPerc`](akimaperc.md) | Specifies the tolerance percentage by which an approximated interpolation point may deviate from the original interpolation point, for Akima subsplines. |
| [`AkimaRange`](akimarange.md) | Specifies the number of neighbor values DIAdem includes when approximating the interpolation points, for Akima subsplines. |
| [`AppEndScript`](appendscript.md) | Specifies which script DIAdem runs when the program ends. |
| [`AppLanguage`](applanguage.md) | Possible spellings: AppLanguage, ApplicationAppLanguage |
| [`ApplicationBitness`](applicationbitness.md) | Specifies whether DIAdem is a 32-bit or a 64-bit version. |
| [`ApplicationChnXYRelationBinding`](applicationchnxyrelationbinding.md) | Specifies whether when plotting xy-channels DIAdem automatically determines the x-channel if it is not explicitly specified. DIAdem saves this setting in the desktop file. |
| [`ApplicationCurveColorsPreset`](applicationcurvecolorspreset.md) | Specifies whether DIAdem uses the user-defined colors for the automatic color selection for new curves. |
| [`ApplicationDefaultScriptLanguage`](applicationdefaultscriptlanguage.md) | Specifies the script language that DIAdem uses by default in DIAdem SCRIPT. |
| [`ApplicationEnablePreviewFeature`](applicationenablepreviewfeature.md) | Specifies whether DIAdem activates soon available functions. |
| [`ApplicationIsHeadless`](applicationisheadless.md) | Specifies whether a DIAdem application was started without using an interface. A DIAdem application is, for example, started in TDM Server without interface, or you start a DIAdem application as Worker object without interface. |
| [`ApplicationIsTDMServer`](applicationistdmserver.md) | Specifies whether a DIAdem application was started in TDM Server. If you test a script containing this variable in the server configuration dialog boxes, this variable also returns TRUE . |
| [`ApplicationLegacyBinaryOperations`](applicationlegacybinaryoperations.md) | Specifies whether bit operations get the same result as in DIAdem versions 2017, 2018, and 2019. In these versions, DIAdem incorrectly included the highest bit in some bit operations. To obtain the same result for bit operations as in DIAdem versions 2017, 2018, and 2019, you must assign the value True to the ApplicationLegacyBinaryOperations variable. DIAdem does not save the ApplicationLegacyBinaryOperations variable of the desktop file. |
| [`ApplicationMaxPathLength`](applicationmaxpathlength.md) | Specifies the maximum possible length of a path. Individual components of the path must not be longer than 260 characters. |
| [`ApplicationName`](applicationname.md) | Specifies an additional text which DIAdem displays in the title bar. |
| [`ApplicationPreviewFeatureCount`](applicationpreviewfeaturecount.md) | Specifies the number of preview features. |
| [`ApplicationPreviewFeatureEnabled`](applicationpreviewfeatureenabled.md) | Specifies whether a preview feature is active or inactive. |
| [`ApplicationPreviewFeatureID`](applicationpreviewfeatureid.md) | Specifies the ID of a preview feature. |
| [`ApplicationPreviewFeatureTitle`](applicationpreviewfeaturetitle.md) | Specifies the title of a preview feature. |
| [`ApplicationPythonInstallOrigin`](applicationpythoninstallorigin.md) | Specifies which Python installation on your computer DIAdem uses to execute Python scripts. |
| [`ApplicationPythonInstallPath`](applicationpythoninstallpath.md) | Valid names: ApplicationPythonInstallPath, PythonInstallPath |
| [`ApplicationTimebaseHighResolution`](applicationtimebasehighresolution.md) | Specifies whether DIAdem creates time channels with a high resolution. Specify this variable before loading data and before assigning variables, because time values in channels and variables otherwise return false data. |
| [`AppMemoryReserve`](appmemoryreserve.md) | Specifies the minimum program memory available for DIAdem as a percentage of the entire memory. This memory space is not used for virtual data management. If this value is exceeded, DIAdem moves the data area to the hard drive. |
| [`ApprAnsatzCoef`](appransatzcoef.md) | Receives the coefficients of an approximation setup function. |
| [`ApprAnsatzFct`](appransatzfct.md) | Specifies the function terms of an approximation. DIAdem combines the selected function terms linear to a setup function. |
| [`ApprAnsatzName`](appransatzname.md) | Receives the names of the selected setup functions for the approximation. |
| [`ApprAnsatzNo`](appransatzno.md) | Receives the number of selected setup functions for an approximation. |
| [`ApprClipCopy`](apprclipcopy.md) | Specifies whether DIAdem copies the approximation results to the clipboard. |
| [`ApprClipType`](apprcliptype.md) | Specifies whether DIAdem transfers the formatted setup function or a table of the coefficients to the clipboard when DIAdem runs an approximation. |
| [`ApprClipValue`](apprclipvalue.md) | Specifies whether DIAdem transfers the approximation results to the clipboard as a value or as a variable reference. |
| [`ApprFctStr`](apprfctstr.md) | Receives the setup function used by an approximation. |
| [`ApprPrecision`](apprprecision.md) | Receives the coefficient of determination of an approximation. |
| [`AppShowCX`](appshowcx.md) |  |
| [`AppShowCY`](appshowcy.md) |  |
| [`AppShowMode`](appshowmode.md) |  |
| [`AppShowName`](appshowname.md) |  |
| [`AppShowX`](appshowx.md) |  |
| [`AppShowY`](appshowy.md) |  |
| [`AppStartScript`](appstartscript.md) | Specifies which script DIAdem runs when the program launches. |
| [`AreaBackColor`](areabackcolor.md) |  |
| [`AreaBackFMode`](areabackfmode.md) |  |
| [`AreaBackFVariant`](areabackfvariant.md) |  |
| [`AreaBackRGB`](areabackrgb.md) |  |
| [`AreaBackRGB2`](areabackrgb2.md) |  |
| [`AreaIso`](areaiso.md) |  |
| [`AreaLimitMode`](arealimitmode.md) | Specifies the x-value range of the area calculation. |
| [`AreaLineClip`](arealineclip.md) |  |
| [`AreaLineColor`](arealinecolor.md) |  |
| [`AreaLineColorRGB`](arealinecolorrgb.md) |  |
| [`AreaLinePt`](arealinept.md) |  |
| [`AreaLineType`](arealinetype.md) |  |
| [`AreaLineWidth`](arealinewidth.md) |  |
| [`AreaShadow`](areashadow.md) |  |
| [`AreaShadowColor`](areashadowcolor.md) |  |
| [`AreaShadowDx`](areashadowdx.md) |  |
| [`AreaShadowDy`](areashadowdy.md) |  |
| [`AreaShadowRGB`](areashadowrgb.md) |  |
| [`AreaSummationMode`](areasummationmode.md) | Determines whether the area calculation includes signs when adding the partial areas. |
| [`ArrowLineColor`](arrowlinecolor.md) |  |
| [`ArrowLineColRGB`](arrowlinecolrgb.md) |  |
| [`ArrowLineWidth`](arrowlinewidth.md) |  |
| [`ArrowLnType`](arrowlntype.md) |  |
| [`ArrowPTX`](arrowptx.md) |  |
| [`ArrowPTY`](arrowpty.md) |  |
| [`ArrowSymbolBegin`](arrowsymbolbegin.md) |  |
| [`ArrowSymbolEnd`](arrowsymbolend.md) |  |
| [`ASCIIOrdLength`](asciiordlength.md) | Specifies the minimum length for ordinal numbers in ASCII block storage. |
| [`ASCIIRealFormat`](asciirealformat.md) | Specifies the format for real numbers in ASCII block storage. |
| [`ASCIISep`](asciisep.md) | Specifies the delimiter for ASCII block storage. If the data is stored blockwise, DIAdem generates a row in the ASCII file for each data block, and separates the single values with the delimiter. |
| [`ASIDelta`](asidelta.md) | Specifies the length of the time interval in ms for the calculation of the moving average in the ASI calculation. |
| [`ASIFilterType`](asifiltertype.md) | Specifies the method of filtering in the ASI calculation. If you do not set this parameter, DIAdem filters with a moving average calculation. |
| [`ASIMax`](asimax.md) | Receives the maximum ASI value. |
| [`ASIVersion`](asiversion.md) | Receives the version number of the ASI calculation routine. |
| [`AudioAutoRepeat`](audioautorepeat.md) | Specifies whether DIAdem restarts the audio output automatically at the end. If the value is TRUE , DIAdem starts the audio output automatically. |
| [`AudioBufferFillEvent`](audiobufferfillevent.md) | Specifies the user command that DIAdem calls when loading new data to the clipboard of the audio output. |
| [`AudioBuffersize`](audiobuffersize.md) | Specifies the number of values DIAdem uses for the buffer of the audio output. If you do not specify this value, DIAdem specifies the size of the buffer automatically. |
| [`AudioEndRow`](audioendrow.md) | Specifies the last channel row at which DIAdem ends the audio output. If you do not specify a value, if you specify a negative value, or if you specify a value larger than the channel length, DIAdem uses the last channel value. |
| [`AudioHandle`](audiohandle.md) | Specifies the handle of the audio output. |
| [`AudioLeftChn`](audioleftchn.md) | Specifies the left channel for the audio output. |
| [`AudioOutMute`](audiooutmute.md) | Specifies whether the sound is on or off. If the value is TRUE , the sound is switched off. |
| [`AudioOutVolume`](audiooutvolume.md) | Specifies the volume of the audio output as a percentage. |
| [`AudioRightChn`](audiorightchn.md) | Specifies the right channel for the audio output. If you do not specify a channel, DIAdem uses the left channel. |
| [`AudioSampleRate`](audiosamplerate.md) | Specifies in Hz the sampling rate DIAdem uses to generate audio signals. If you specify 0 or no value, DIAdem tries to specify the sampling rate from the properties wf_xunit_string and wf_increment . If these properties are missing or in an incorrect unit, DIAdem uses the value 44.1 kHz. |
| [`AudioStartRow`](audiostartrow.md) | Specifies the first channel row from where DIAdem starts the audio output. If you do not specify a value or if you specify a negative value, DIAdem uses the first value of the channel. |
| [`AudioStartSuspended`](audiostartsuspended.md) | Specifies that the audio output does not start directly. Use the commands AudioOutSuspend and AudioOutResume to stop or to continue the audio output. |
| [`AutEdCheckTime`](autedchecktime.md) |  |
| [`AutEdExt`](autedext.md) | Specifies the filename extension of the file currently open in the script editor. |
| [`AutEdFileType`](autedfiletype.md) | Specifies the file type of a new file in the script editor. |
| [`AutEdModifiedIs`](autedmodifiedis.md) | Specifies whether the current file was changed in the script editor. |
| [`AutEdName`](autedname.md) | Specifies the filename of the file currently open in the script editor. |
| [`AutEdNoASCFiles`](autednoascfiles.md) |  |
| [`AutEdNoAUTFiles`](autednoautfiles.md) |  |
| [`AutEdNoElseFiles`](autednoelsefiles.md) |  |
| [`AutEdNoFiles`](autednofiles.md) | Specifies the number of files open in the script editor. |
| [`AutEdNoLSTFiles`](autednolstfiles.md) |  |
| [`AutEdNoVASFiles`](autednovasfiles.md) |  |
| [`AutEdNoVBSFiles`](autednovbsfiles.md) |  |
| [`AutEdSyntax`](autedsyntax.md) | Specifies the syntax of the loaded file. |
| [`AutEdTabIndex`](autedtabindex.md) | Specifies the index of a file that is open in the script editor. |
| [`AutEdTabModified`](autedtabmodified.md) |  |
| [`AutEdTabName`](autedtabname.md) | Specifies the name you use to save a file in the script editor. By default the AutEdTabName variable contains the name of the loaded file. |
| [`AutEdText`](autedtext.md) |  |
| [`AutEdTypeLibId`](autedtypelibid.md) | Specifies the identification of the type library you register in DIAdem. |
| [`AutEdTypeLibVer`](autedtypelibver.md) | Specifies the type library version you register in DIAdem. |
| [`AutEdWSDeskfile`](autedwsdeskfile.md) | Specifies the default file for the workspace of the DIAdem SCRIPT panel. |
| [`AutoAbort`](autoabort.md) | Specifies whether you can abort scripts with <Esc>. |
| [`AutoActFile`](autoactfile.md) | Specifies the name and the path of the script file currently running. Use the variables CurrentScriptName nd CurrentScriptPath instead of this variable. |
| [`AutoActLine`](autoactline.md) |  |
| [`AutoActName`](autoactname.md) | Specifies the name of the script file currently running. Use the CurrentScriptName variable instead of this variable. |
| [`AutoActPath`](autoactpath.md) | Specifies the path of the script file currently running. Use the CurrentScriptPath variable instead of this variable. |
| [`AutoCnd`](autocnd.md) |  |
| [`AutoDrvLibr`](autodrvlibr.md) |  |
| [`AutoDrvUser`](autodrvuser.md) | Valid names: AutoDrvUser, AutoDrv |
| [`AutoEcho`](autoecho.md) | Specifies whether DIAdem displays messages in the status bar while the script runs. |
| [`AutoFile`](autofile.md) | Specifies the name of a script file. |
| [`AutoIgnoreError`](autoignoreerror.md) |  |
| [`AutoLstFile`](autolstfile.md) | Specifies the name of a list file for a Serial evaluation . |
| [`AutoMsg`](automsg.md) | Specifies a message text that DIAdem displays when a script aborts. |
| [`AutoStartLev`](autostartlev.md) | Specifies the current nesting depths of scripts. |
| [`AutoStartLevMax`](autostartlevmax.md) | Specifies the maximum nesting depths of scripts. |
| [`AutoTeachMode`](autoteachmode.md) | Specifies whether the recording mode is active. |
| [`AutoTimeChn`](autotimechn.md) | Specifies whether DIAdem uses the first channel of a channel group as the time channel or whether you specify the time channel. If the value is TRUE , DIAdem uses the first channel of a channel group as the time channel. If the input channels are waveform channels, DIAdem uses the time part of the waveform. |
| [`AWFiltType`](awfilttype.md) | Specifies the frequency weighting filter for time-related body and hand-arm vibrations in accordance with ISO 2631-1 and VDI 2057-1,2. |
| [`AWMTVV`](awmtvv.md) | Specifies the maximum of the floating RMS in a frequency-weighted acceleration. |
| [`AWRedFactor`](awredfactor.md) | Specifies how many values DIAdem groups into one result value in a frequency-weighted acceleration. |
| [`AWRMSRunning`](awrmsrunning.md) | Specifies whether DIAdem calculates the floating RMS for the frequency-weighted acceleration. |
| [`AWRMSTime`](awrmstime.md) | Specifies the time constant for mean calculations, in seconds. |
| [`AxisNoMax`](axisnomax.md) | Specifies the maximum number of subaxes you can define in one REPORT axis system. |
| [`B1`](b1.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B10`](b10.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B2`](b2.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B3`](b3.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B4`](b4.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B5`](b5.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B6`](b6.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B7`](b7.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B8`](b8.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`B9`](b9.md) | Specifies the contents of the Boolean type single-value auxiliary variable |
| [`BarManager`](barmanager.md) | Specifies the BarManager object that provides access to the subobjects, methods, and properties for bar configuration. |
| [`BrIC`](bric.md) | Receives the result of a BrIC calculation. |
| [`BrICVersion`](bricversion.md) | Receives the version number of the BrIC calculation routine. |
| [`BulkDataLoadingMode`](bulkdataloadingmode.md) | Specifies when DIAdem loads bulk data into the Data Portal. |
| [`BusLogAutoConvert`](buslogautoconvert.md) | Specifies whether DIAdem automatically converts an XNET-TDMS file or an MDF4 bus logfile when loading. |
| [`BusLogConvertInitFile`](buslogconvertinitfile.md) | Specifies the name of the bus-database configuration. |
| [`BusLogToTDM`](buslogtotdm.md) | Specifies the BusLogToTDM object that facilitates the conversion of bus log files into a TDM file. |
| [`CalcDuration`](calcduration.md) | Specifies the duration of the user-defined time-at-level calculation. |
| [`CalcFormat`](calcformat.md) | Specifies the prescribed format for the coefficients. |
| [`CalcInjury`](calcinjury.md) | Specifies whether DIAdem calculates the limit curve for the time-at-level. |
| [`CalcQuantityBased`](calcquantitybased.md) | Specifies whether DIAdem executes the calculations quantity-based in DIAdem ANALYSIS and in the Calculator. |
| [`CalcSteps`](calcsteps.md) | Specifies the number of steps for the user-defined time-at-level calculation. |
| [`CalculateResultUnit`](calculateresultunit.md) | Specifies the result unit of a formula calculation that you executed with the Calculate command. |
| [`CalculateSymbols`](calculatesymbols.md) | Valid names: CalculateSymbols, CSym |
| [`CalculateTargetUnit`](calculatetargetunit.md) | Specifies the unit symbol for the result of the calculation. If you specify the "Default" value, DIAdem uses the matching default unit of the active unit set of the result channel. If you specify an empty string, DIAdem specifies the unit symbol. |
| [`CalculateValues`](calculatevalues.md) | Valid names: CalculateValues, CVal |
| [`CalculationSet`](calculationset.md) | Specifies the CalculationSet object, which provides access to the subobjects, methods, and properties for working with calculation templates. |
| [`CalcXChn`](calcxchn.md) | Specifies the data channel containing the x-values of the signal. |
| [`CalcYChn`](calcychn.md) | Specifies the data channels containing the y-values of the signal. |
| [`CANToTDM`](cantotdm.md) | Specifies the BusLogToTDM object that facilitates the conversion of bus log files into a TDM file. |
| [`CClassMeth`](cclassmeth.md) | Specifies the classification procedure for a compound classification. |
| [`CCR`](ccr.md) | Specifies the number of the current cycle when a calculation template is executed in serial calculation. |
| [`CFCFiltType`](cfcfilttype.md) | Specifies the filtering characteristic with specific limit frequencies and tolerance widths for lowpass filters. |
| [`CFCFreeValue`](cfcfreevalue.md) | Specifies the filter class when the CFC filtering is non-standardized. If you do not specify the CFCFreeValue variable, DIAdem uses the value 0 . |
| [`CFCPreEventType`](cfcpreeventtype.md) | Specifies how DIAdem extends the input data at the starting point and the end point of the signal, to eliminate transient response in the filter. If you do not specify the variable CFCPreEventType , DIAdem uses the value ZeroMagnitude . |
| [`CH`](ch.md) | Specifies the channel for calculations with the calculator. |
| [`ChannelList`](channellist.md) | Specifies a channel list as a vector in the script environment. |
| [`ChannelNames`](channelnames.md) | Specifies the names of the channels. |
| [`CharMapFont`](charmapfont.md) | Specifies the name of the font in the dialog box of the character table. |
| [`CharMapFontEnabled`](charmapfontenabled.md) | Specifies whether you can select the font in the dialog box of the character table. |
| [`CharMapText`](charmaptext.md) | Receives the character selected in the character table. |
| [`CHD`](chd.md) | Valid names: CHD, ChnVal |
| [`ChDWfX`](chdwfx.md) | Specifies an x-value of a waveform channel. The first index specifies the channel row, the second index specifies the waveform channel with the channel name or with the channel number. |
| [`ChDX`](chdx.md) |  |
| [`CHF`](chf.md) | Valid names: CHF, ChnFlag |
| [`ChnArg1`](chnarg1.md) | Specifies a channel. |
| [`ChnArg2`](chnarg2.md) | Specifies a further channel. |
| [`ChnAttrInt1`](chnattrint1.md) |  |
| [`ChnAttrInt2`](chnattrint2.md) |  |
| [`ChnAttrInt3`](chnattrint3.md) |  |
| [`ChnAttrInt4`](chnattrint4.md) |  |
| [`ChnAttrInt5`](chnattrint5.md) |  |
| [`ChnAttrTxt1`](chnattrtxt1.md) |  |
| [`ChnAttrTxt2`](chnattrtxt2.md) |  |
| [`ChnAttrVal1`](chnattrval1.md) |  |
| [`ChnAttrVal2`](chnattrval2.md) |  |
| [`ChnAttrVal3`](chnattrval3.md) |  |
| [`ChnAttrVal4`](chnattrval4.md) |  |
| [`ChnAttrVal5`](chnattrval5.md) |  |
| [`ChnAttrVal6`](chnattrval6.md) | Valid names: ChnAttrVal6, ASCIILine |
| [`ChnBaseName`](chnbasename.md) | Specifies the base name of the new channels, which is used when the channels are converted from an array. |
| [`ChnBegin`](chnbegin.md) | Specifies the start value when DIAdem generates a channel. |
| [`ChnCharacteristicsUpdate`](chncharacteristicsupdate.md) | Specifies whether DIAdem calculates the characteristic values when loading defined criteria automatically according to specific criteria or not. The default value is FALSE , which specifies that DIAdem does not calculate the characteristic values. |
| [`ChnComment`](chncomment.md) | Valid names: ChnComment, CC |
| [`ChnCommentOver`](chncommentover.md) | Specifies whether DIAdem overwrites existing channel comments with calculation operations. |
| [`ChnConcatenateChannelsByName`](chnconcatenatechannelsbyname.md) | Specifies that DIAdem concatenates channels with the name ( TRUE ) or the index ( FALSE ) of the individual groups. |
| [`ChnConcatenateInPlace`](chnconcatenateinplace.md) | Specifies whether DIAdem overwrites the values of the base channel or channels with results. |
| [`ChnConcatenateMarkBoundaries`](chnconcatenatemarkboundaries.md) | Specifies that DIAdem inserts a separator after each channel to make the original channels visible. DIAdem inserts NoValue for numeric channels and the following character: .---.-. for text channels. |
| [`ChnConcatenateRestoreWaveform`](chnconcatenaterestorewaveform.md) | Specifies that DIAdem saves the result channels like the input channels as waveform channels if possible. This requires the new time axis of each waveform channel to be continually equidistant. |
| [`ChnConvertMode`](chnconvertmode.md) | Specifies whether you convert numeric channels to waveform channels or vice versa. |
| [`ChnCRedIP`](chncredip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result values of the reducing classification. The default value is FALSE , which specifies that DIAdem does not overwrite the input channels. |
| [`ChnDataFileName`](chndatafilename.md) | Valid names: ChnDataFileName, CFN |
| [`ChnDataFilePath`](chndatafilepath.md) | Valid names: ChnDataFilePath, CFP |
| [`ChnDataSaveMode`](chndatasavemode.md) | Specifies the storage mode of the channel. |
| [`ChnDataStyle`](chndatastyle.md) | When saving channel data to a DAT, TDMS, or TDM file, DIAdem prefers to use this data type or a more suitable one. |
| [`ChnDataType`](chndatatype.md) | Specifies the preferred channel type with which DIAdem saves channels. |
| [`ChnDiffKeepChnLength`](chndiffkeepchnlength.md) | Specifies whether the channel length of the result channels and the input channels is the same during the differentiation. |
| [`ChnDim`](chndim.md) | Valid names: ChnDim, CD |
| [`ChnEventList1`](chneventlist1.md) | Receives the result of a search or the result of the logical operation of several searches. |
| [`ChnEventList2`](chneventlist2.md) | Receives the result of a search or the result of the logical operation of several searches. |
| [`ChnEventListIndex`](chneventlistindex.md) | Specifies the index of the event. If the index is not specified or if Null is specified, DIAdem includes all events. |
| [`ChnEventResultList`](chneventresultlist.md) | Receives the search result or its operator. |
| [`ChnFindStartIdx`](chnfindstartidx.md) | Specifies the row number at which DIAdem begins checking the data channel for a condition. By default DIAdem checks the data channel in the command ChnFind from the first row and in the command ChnFindReverse from the last row. |
| [`ChnFormat`](chnformat.md) |  |
| [`ChnGroup`](chngroup.md) |  |
| [`ChnHistory`](chnhistory.md) |  |
| [`ChnIndex`](chnindex.md) |  |
| [`ChnIsIntern`](chnisintern.md) | Specifies whether the channel is an internal channel. |
| [`ChnLength`](chnlength.md) | Valid names: ChnLength, CL |
| [`ChnLengthMax`](chnlengthmax.md) |  |
| [`ChnList`](chnlist.md) | Specifies one or more channels. |
| [`ChnList1`](chnlist1.md) | Specifies one or more channels. |
| [`ChnList2`](chnlist2.md) | Specifies one or more channels. |
| [`ChnMonotonyKey`](chnmonotonykey.md) |  |
| [`ChnMSortIP`](chnmsortip.md) | Specifies whether DIAdem overwrites the values of the input channels with the sorting result values. The default value is FALSE , which specifies that DIAdem does not overwrite the input channels. |
| [`ChnName`](chnname.md) | Valid names: ChnName, CN |
| [`ChnNameExt`](chnnameext.md) |  |
| [`ChnNo`](chnno.md) |  |
| [`ChnNoMax`](chnnomax.md) | Specifies the current number of channels. You also can use the object-oriented interface to access internal data. The property Count for Channels replaces the variable ChnNoMax . |
| [`ChnNoStr`](chnnostr.md) | Valid names: ChnNoStr, ChnNumberString |
| [`ChnNoStr1`](chnnostr1.md) |  |
| [`ChnNoStr2`](chnnostr2.md) |  |
| [`ChnNoStr3`](chnnostr3.md) |  |
| [`ChnNovIP`](chnnovip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result channels of NoValue processing. The default value is FALSE , which specifies that DIAdem does not overwrite the input channels. |
| [`ChnNovKey`](chnnovkey.md) | Specifies whether a channel contains NoValues. |
| [`ChnOffsetMode`](chnoffsetmode.md) | Specifies the type of offset correction DIAdem uses. |
| [`ChnOffsetValue`](chnoffsetvalue.md) | Specifies the number of values that DIAdem averages or the free offset that DIAdem adds to the individual channel values. |
| [`ChnOrder`](chnorder.md) |  |
| [`ChnPairMode`](chnpairmode.md) | Specifies whether the numeric channel pair is real and imaginary part or magnitude and phase. In non-quantity-based calculations , DIAdem expects the phase in rad . |
| [`ChnPropCount`](chnpropcount.md) |  |
| [`ChnRangeLimitLower`](chnrangelimitlower.md) | Specifies the lower limit to restrict a data channel. |
| [`ChnRangeLimitUpper`](chnrangelimitupper.md) | Specifies the upper limit to restrict a data channel. |
| [`ChnResult`](chnresult.md) | Contains the result channel or result channels. The result is ElementList <Data> type. |
| [`ChnRow`](chnrow.md) | Specifies the row number in a channel. |
| [`ChnScaleFactor`](chnscalefactor.md) | Specifies the scaling factor. |
| [`ChnScaleOffset`](chnscaleoffset.md) | Specifies the scaling offset. |
| [`ChnStartVal`](chnstartval.md) | Specifies the start value or the offset of a channel. |
| [`ChnStep`](chnstep.md) | Specifies the step width for generating equidistant channel values. |
| [`ChnStepWidth`](chnstepwidth.md) | Specifies the step width or the calibration factor of the channel. |
| [`ChnTargetKey`](chntargetkey.md) |  |
| [`ChnTargetType`](chntargettype.md) | Specifies the type of the result channel. |
| [`ChnTimeConversionMode`](chntimeconversionmode.md) | Determines whether you convert a numeric channel to a time channel or vice versa. |
| [`ChnUnitOperator`](chnunitoperator.md) | Specifies the operator. |
| [`ChnValFormat`](chnvalformat.md) |  |
| [`ChnValMax`](chnvalmax.md) | Valid names: ChnValMax, CMax |
| [`ChnValMin`](chnvalmin.md) | Valid names: ChnValMin, CMin |
| [`ChnValueDataType`](chnvaluedatatype.md) |  |
| [`ChnVisible`](chnvisible.md) |  |
| [`ChnWfKey`](chnwfkey.md) |  |
| [`ChoosedColor`](choosedcolor.md) | Specifies the RGB color value. |
| [`CHT`](cht.md) |  |
| [`ChV`](chv.md) |  |
| [`CircleBkColor`](circlebkcolor.md) |  |
| [`CircleBkColRGB`](circlebkcolrgb.md) |  |
| [`CircleClipCopy`](circleclipcopy.md) | Specifies whether DIAdem transfers the results of the circle approximation to the clipboard. |
| [`CircleClipValue`](circleclipvalue.md) | Specifies whether DIAdem transfers the circle approximation results to the clipboard as a value or as a variable reference. |
| [`CircleConcCmci`](circleconccmci.md) | Receives the characteristic values of the concentric circumcircle. |
| [`CircleConcInci`](circleconcinci.md) | Receives the characteristic values of the concentric incircle. |
| [`CircleFctStr`](circlefctstr.md) | Specifies the format that DIAdem uses to copy the results of the circle approximation to the clipboard. |
| [`CircleIso`](circleiso.md) |  |
| [`CircleLnColor`](circlelncolor.md) |  |
| [`CircleLnColRGB`](circlelncolrgb.md) |  |
| [`CircleLnType`](circlelntype.md) |  |
| [`CircleLnWidth`](circlelnwidth.md) |  |
| [`CircleMaxInci`](circlemaxinci.md) | Receives the characteristic values of the maximum incircle. |
| [`CircleMinCmci`](circlemincmci.md) | Receives the characteristic values of the minimum circumcircle. |
| [`CirclePrecision`](circleprecision.md) | Specifies the relative precision of the incircle and circumcircle calculation as a percentage of the radius of the regression circle. |
| [`CirclePt`](circlept.md) |  |
| [`CircleRegr`](circleregr.md) | Receives the characteristic values of the regression circle. |
| [`CircleResol`](circleresol.md) | Specifies the number of points per approximation circle. |
| [`CircleType`](circletype.md) | Specifies the approximation circles to be calculated. |
| [`ClassBegin`](classbegin.md) | Specifies the lower limit of the first class interval. |
| [`ClassBegin1`](classbegin1.md) | Specifies the lower limit of the first class interval for the first signal. |
| [`ClassBegin2`](classbegin2.md) | Specifies the lower limit of the first class interval for the second signal. |
| [`ClassChn`](classchn.md) | Specifies which data channel defines the non equidistant class limits. |
| [`ClassDontUseNV`](classdontusenv.md) | Specifies whether DIAdem ignores or replaces NoValues in a reducing classification. The default value is FALSE , which specifies that DIAdem does not replace NoValues. |
| [`ClassEnd`](classend.md) | Specifies the upper limit of the last class interval. |
| [`ClassEnd1`](classend1.md) | Specifies the upper limit of the last class interval for the first signal. |
| [`ClassEnd2`](classend2.md) | Specifies the upper limit of the last class interval for the second signal. |
| [`ClassMeth1`](classmeth1.md) | Valid names: ClassMeth1, ClassRangeMeth |
| [`ClassMeth2`](classmeth2.md) | Specifies how DIAdem specifies the class limits. |
| [`ClassNo`](classno.md) | Specifies the number of classes to generate. |
| [`ClassNo1`](classno1.md) | Specifies the number of classes to generate for the first signal. |
| [`ClassNo2`](classno2.md) | Specifies the number of classes to generate for the second signal. |
| [`ClassNVReplace`](classnvreplace.md) | Specifies the value with which DIAdem replaces NoValues in a reducing classification. The default value of the ClassNVReplace variable is 0 . |
| [`ClassRange`](classrange.md) | Specifies how many values DIAdem uses for calculating the maximum value. |
| [`ClassRangeWidth`](classrangewidth.md) | Specifies the difference between the class beginning of the smallest class and the class end of the greatest class. |
| [`ClassRangeWidth1`](classrangewidth1.md) | Specifies the difference between the class begin and the class end for the first signal. |
| [`ClassRangeWidth2`](classrangewidth2.md) | Specifies the difference between the class begin and the class end for the second signal. |
| [`ClassRed2Params`](classred2params.md) | Specifies whether the reducing classification works with one x-channel or with two x-channels. If the value is TRUE , DIAdem works with two x-channel. |
| [`ClassRefLine`](classrefline.md) | Specifies the zero line that divides the signal into positive and negative sections. |
| [`ClassRefLineY`](classrefliney.md) | Specifies the zero line that divides the signal into positive and negative sections. |
| [`ClassSingleMeth`](classsinglemeth.md) | Specifies the classification method for single classification. |
| [`ClassWidth`](classwidth.md) | Specifies the width of the class interval. |
| [`ClassWidth1`](classwidth1.md) | Specifies the width of the class interval for the first signal. |
| [`ClassWidth2`](classwidth2.md) | Specifies the width of the class interval for the second signal. |
| [`ClassXRed`](classxred.md) | Specifies the type of data reduction. |
| [`ClpSource`](clpsource.md) | Specifies one or more channels. |
| [`ClpSourceData`](clpsourcedata.md) | Specifies which group name or group index, or array with the group names DIAdem copies. |
| [`ClpTarget`](clptarget.md) | Specifies the channel which receives the first inserted channel. |
| [`CmdNoDialogDisp`](cmdnodialogdisp.md) | Specifies whether DIAdem suppresses the display of dialog boxes. |
| [`CmdNoErrorDisp`](cmdnoerrordisp.md) | Specifies whether DIAdem suppresses the display of error messages. |
| [`CmdNoInfoDisp`](cmdnoinfodisp.md) | Specifies whether DIAdem suppresses the display of information messages. |
| [`CmdNoMsgDisp`](cmdnomsgdisp.md) | Specifies whether DIAdem suppresses the display of messages and dialog boxes. |
| [`CmdNoWarningDisp`](cmdnowarningdisp.md) | Specifies whether DIAdem suppresses the display of warnings. |
| [`CmtArrowEndPTX`](cmtarrowendptx.md) |  |
| [`CmtArrowEndPTY`](cmtarrowendpty.md) |  |
| [`CmtArrowLnColor`](cmtarrowlncolor.md) |  |
| [`CmtArrowLnColRGB`](cmtarrowlncolrgb.md) |  |
| [`CmtArrowLnType`](cmtarrowlntype.md) |  |
| [`CmtArrowLnWidth`](cmtarrowlnwidth.md) |  |
| [`CmtArrowPTPos`](cmtarrowptpos.md) |  |
| [`CmtArrowStartPTX`](cmtarrowstartptx.md) |  |
| [`CmtArrowStartPTY`](cmtarrowstartpty.md) |  |
| [`CmtArrowSymbBeg`](cmtarrowsymbbeg.md) |  |
| [`CmtArrowSymbEnd`](cmtarrowsymbend.md) |  |
| [`CmtFrameBackFMode`](cmtframebackfmode.md) |  |
| [`CmtFrameBackFVariant`](cmtframebackfvariant.md) |  |
| [`CmtFrameBkColor`](cmtframebkcolor.md) |  |
| [`CmtFrameBkColRGB`](cmtframebkcolrgb.md) |  |
| [`CmtFrameBkColRGB2`](cmtframebkcolrgb2.md) |  |
| [`CmtFrameLnColor`](cmtframelncolor.md) |  |
| [`CmtFrameLnColRGB`](cmtframelncolrgb.md) |  |
| [`CmtFrameLnType`](cmtframelntype.md) |  |
| [`CmtFrameLnWidth`](cmtframelnwidth.md) |  |
| [`CmtFramePT`](cmtframept.md) |  |
| [`CmtTxt`](cmttxt.md) |  |
| [`CmtTxtAlignment`](cmttxtalignment.md) |  |
| [`CmtTxtBold`](cmttxtbold.md) |  |
| [`CmtTxtColor`](cmttxtcolor.md) |  |
| [`CmtTxtColorRGB`](cmttxtcolorrgb.md) |  |
| [`CmtTxtFont`](cmttxtfont.md) |  |
| [`CmtTxtItal`](cmttxtital.md) |  |
| [`CmtTxtSize`](cmttxtsize.md) |  |
| [`CmtTxtStrOut`](cmttxtstrout.md) |  |
| [`CmtTxtUndl`](cmttxtundl.md) |  |
| [`ColorLst`](colorlst.md) | Specifies a list of colors. |
| [`CommonDocumentsPath`](commondocumentspath.md) | Specifies the user folder where you save common files. A typical path is c:\Users\Public\Documents\National Instruments\ <Version> . |
| [`CommonTimeFormat`](commontimeformat.md) | Specifies the format string to be checked. Receives a universal time format after the CommonTimeFormatCheck command is called. |
| [`ConfLibrPath`](conflibrpath.md) | Valid names: ConfLibrPath, UsrCnfLibrPath |
| [`ConfReadPath`](confreadpath.md) | Valid names: ConfReadPath, UsrCnfReadPath |
| [`ConfWritePath`](confwritepath.md) | Valid names: ConfWritePath, UsrCnfWritePath |
| [`ConstTransfInX`](consttransfinx.md) |  |
| [`ConstTransfInY`](consttransfiny.md) |  |
| [`ConstTransfOutX`](consttransfoutx.md) |  |
| [`ConstTransfOutY`](consttransfouty.md) |  |
| [`CorrelBothSided`](correlbothsided.md) | Specifies that DIAdem calculates the correlation on both sides. This way DIAdem includes the displacement in the positive as well as in the negative direction in order to find the displacement with the smallest absolute value. |
| [`CorrelNormalize`](correlnormalize.md) | Specifies that DIAdem normalizes the correlation results ranging from -1 to +1. |
| [`CorrelType`](correltype.md) | Specifies whether DIAdem runs the calculation in the frequency domain or the time domain. |
| [`CorrelVal`](correlval.md) | Specifies the maximum shift of the signal, as a percentage of the channel length, for the correlation in the time domain. |
| [`CorridorCheck`](corridorcheck.md) | Specifies whether the values are all within the specified range. |
| [`CorridorCheckTIdx`](corridorchecktidx.md) | Receives the number of the first point outside the given range. |
| [`CorridorCheckVersion`](corridorcheckversion.md) | Valid names: PulseLimitVer, PulseLimitVersion |
| [`CorridorOffsetXType`](corridoroffsetxtype.md) | Specifies whether the distance of the parallel curves to the input signal in x-direction is specified in absolute or relative numbers. |
| [`CorridorOffsetXValue`](corridoroffsetxvalue.md) | Specifies the distance of the parallel curves to the input signal in x-direction. |
| [`CorridorOffsetYType`](corridoroffsetytype.md) | Specifies whether the distance of the parallel curves to the input signal in y-direction is specified in absolute or relative numbers. |
| [`CorridorOffsetYValue`](corridoroffsetyvalue.md) | Specifies the distance of the parallel curves to the input signal in y-direction. |
| [`CorridorPointsPerArc`](corridorpointsperarc.md) | Specifies the number of extra curve partitions at the local extreme values of the input signal. A greater number of partitions creates smoother curves but also needs more computing time. |
| [`CorridorPointsPerLine`](corridorpointsperline.md) | Specifies the number of extra partitions between two points of the input signal. A greater number of partitions creates curves that adjust better to the signal, especially with greater distances, but this also needs more computing time. |
| [`CPUAffinity`](cpuaffinity.md) | Receives the names of the processors that DIAdem uses. |
| [`CrashDummyConst`](crashdummyconst.md) | Specifies the deformation constant (chest depth) of the dummy in millimeters. |
| [`CreateNewChannel`](createnewchannel.md) | Specifies whether DIAdem saves the result in a new channel ( TRUE ) or whether DIAdem overwrites the input channel with the result ( FALSE ). |
| [`CryptFile`](cryptfile.md) | Specifies which file to encrypt. You can also specify the path and the filename extension. |
| [`CurrAbsValue`](currabsvalue.md) | Possible notations: CurrAbsValue, CAV |
| [`CurrAxisName`](curraxisname.md) | Specifies the axis name DIAdem uses when drawing. |
| [`CurrAxisNo`](curraxisno.md) | Possible spellings: CurrAxisNo, CAxN |
| [`CurrChnIdx`](currchnidx.md) | Valid names: CurrChnIdx, CCI |
| [`CurrChnNo`](currchnno.md) | Possible spellings: CurrChnNo, CCN, CurrChnID, CCID |
| [`CurrDate`](currdate.md) | Specifies the current date. |
| [`CurrDateTime`](currdatetime.md) | Specifies the current date and the current time. |
| [`CurrDateTimeReal`](currdatetimereal.md) | Specifies the current date and the current time as a numeric value. |
| [`CurrDXValue`](currdxvalue.md) | Specifies the current dx value DIAdem uses when drawing. |
| [`CurrDYValue`](currdyvalue.md) | Specifies the current dy-value DIAdem uses when drawing. |
| [`CurrDZValue`](currdzvalue.md) | Specifies the current dz-value DIAdem uses when drawing. |
| [`CurrentScriptName`](currentscriptname.md) | Specifies the name of the script file currently running. |
| [`CurrentScriptPath`](currentscriptpath.md) | Specifies the path of the script file currently running. |
| [`CurrFormatValue`](currformatvalue.md) | Valid names: CurrFormatValue, CFV |
| [`CurrGroupIdx`](currgroupidx.md) | Valid names: CurrGroupIdx, CGI |
| [`CurrRelValue`](currrelvalue.md) | Possible notations: CurrRelValue, CRV |
| [`CurrTime`](currtime.md) | Specifies the current time. |
| [`CurrVal1Idx`](currval1idx.md) | Possible spellings: CurrVal1Idx, CV1I |
| [`CurrValIdx`](currvalidx.md) | Possible spellings: CurrValIdx, CVI |
| [`CurrX1Value`](currx1value.md) | Specifies the current 1x value DIAdem uses when drawing. |
| [`CurrXChnIdx`](currxchnidx.md) | Possible spellings: CurrXChnIdx, CXCI |
| [`CurrXChnName`](currxchnname.md) | Possible syntax: CurrXChnName, CXCName |
| [`CurrXChnNo`](currxchnno.md) | Possible spellings: CurrXChnNo, CXCN |
| [`CurrXChnReference`](currxchnreference.md) | Specifies the current channel reference of the x-channel of the curve, which DIAdem plots. |
| [`CurrXGroupIdx`](currxgroupidx.md) | Possible spellings: CurrXGroupIdx, CXGI |
| [`CurrXGroupName`](currxgroupname.md) | Possible spellings: CurrXGroupName, CXGN |
| [`CurrXValue`](currxvalue.md) | Specifies the current x-value DIAdem uses when drawing. |
| [`CurrY1Value`](curry1value.md) | Specifies the current y1-value DIAdem uses when drawing. |
| [`CurrYChnIdx`](currychnidx.md) | Valid names: CurrYChnIdx, CYCI |
| [`CurrYChnName`](currychnname.md) | Possible syntax: CurrYChnName, CYCName |
| [`CurrYChnNo`](currychnno.md) | Possible spellings: CurrYChnNo, CYCN |
| [`CurrYChnReference`](currychnreference.md) | Specifies the current channel reference of the y-channel of the curve, which DIAdem plots. |
| [`CurrYGroupIdx`](currygroupidx.md) | Possible spellings: CurrYGroupIdx, CYGI |
| [`CurrYGroupName`](currygroupname.md) | Possible spellings: CurrYGroupName, CYGN |
| [`CurrYValue`](curryvalue.md) | Specifies the current y-value DIAdem uses when drawing. |
| [`CurrZ1Value`](currz1value.md) | Specifies the current z1-value DIAdem uses when drawing. |
| [`CurrZChnIdx`](currzchnidx.md) | Possible spellings: CurrZChnIdx, CZCI |
| [`CurrZChnName`](currzchnname.md) | Possible syntax: CurrZChnName, CZCName |
| [`CurrZChnNo`](currzchnno.md) | Possible spellings: CurrZChnNo, CZCN |
| [`CurrZChnReference`](currzchnreference.md) | Specifies the current channel reference of the z-channel of the curve, which DIAdem plots. |
| [`CurrZGroupIdx`](currzgroupidx.md) | Possible spellings: CurrZGroupIdx, CZGI |
| [`CurrZGroupName`](currzgroupname.md) | Possible spellings: CurrZGroupName, CZGN |
| [`CurrZValue`](currzvalue.md) | Specifies the current z-value DIAdem uses when drawing. |
| [`CurveNoMax`](curvenomax.md) | Valid names: CurveNoMax, CurveIdentNoMax |
| [`CurveObject`](curveobject.md) | Specifies the curve that contains the curve section. |
| [`CurveSnippetSize`](curvesnippetsize.md) | Specifies the length of the curve section. Specify the length as the number of spaces which DIAdem replaces with the curve section. |
| [`CurveTransfCFG`](curvetransfcfg.md) |  |
| [`CurveTransfInX`](curvetransfinx.md) | Valid names: CurveTransfInX, CTrInX |
| [`CurveTransfInY`](curvetransfiny.md) | Valid names: CurveTransfInY, CTrInY |
| [`CurveTransfInY1`](curvetransfiny1.md) | Valid names: CurveTransfInY1, CTrInY1 |
| [`CurveTransfOutX`](curvetransfoutx.md) | Valid names: CurveTransfOutX, CTrOutX |
| [`CurveTransfOutY`](curvetransfouty.md) | Valid names: CurveTransfOutY, CTrOutY |
| [`CurveTransfOutY1`](curvetransfouty1.md) | Valid names: CurveTransfOutY1, CTrOutY1 |
| [`CustomHelpFilename`](customhelpfilename.md) | Valid names: CustomHelpFilename, WinHelpFile |
| [`CustomHelpURL`](customhelpurl.md) | Valid names: CustomHelpURL, WinHelpTopic |
| [`CycleVal`](cycleval.md) | Specifies the frequency for value classification. |
| [`D2AxisBackColor`](d2axisbackcolor.md) |  |
| [`D2AxisBackColRGB`](d2axisbackcolrgb.md) |  |
| [`D2AxisBackColRGB2`](d2axisbackcolrgb2.md) |  |
| [`D2AxisBackFMode`](d2axisbackfmode.md) |  |
| [`D2AxisBackFVariant`](d2axisbackfvariant.md) |  |
| [`D2AxisBottom`](d2axisbottom.md) |  |
| [`D2AxisColor`](d2axiscolor.md) | Valid names: D2AxisColor, D2AxisFrameColor |
| [`D2AxisColorRGB`](d2axiscolorrgb.md) | Valid names: D2AxisColorRGB, D2AxisFrameCoRGB |
| [`D2AxisCTransform`](d2axisctransform.md) |  |
| [`D2AxisDisp`](d2axisdisp.md) |  |
| [`D2AxisDispType`](d2axisdisptype.md) |  |
| [`D2AxisGridColor`](d2axisgridcolor.md) |  |
| [`D2AxisGridColRGB`](d2axisgridcolrgb.md) |  |
| [`D2AxisGridDotsPerTick`](d2axisgriddotspertick.md) |  |
| [`D2AxisGridInterv`](d2axisgridinterv.md) |  |
| [`D2AxisGridType`](d2axisgridtype.md) |  |
| [`D2AxisHide`](d2axishide.md) |  |
| [`D2AxisIndividCol`](d2axisindividcol.md) |  |
| [`D2AxisIsoDisp`](d2axisisodisp.md) |  |
| [`D2AxisLeft`](d2axisleft.md) |  |
| [`D2AxisLineWidth`](d2axislinewidth.md) |  |
| [`D2AxisOffsetY`](d2axisoffsety.md) |  |
| [`D2AxisRight`](d2axisright.md) |  |
| [`D2AxisScaled`](d2axisscaled.md) |  |
| [`D2AxisScaledIn`](d2axisscaledin.md) |  |
| [`D2AxisSegmentChnX`](d2axissegmentchnx.md) |  |
| [`D2AxisSegmentChnXName`](d2axissegmentchnxname.md) |  |
| [`D2AxisSegmentChnY`](d2axissegmentchny.md) |  |
| [`D2AxisSegmentChnYName`](d2axissegmentchnyname.md) |  |
| [`D2AxisSegmentColor`](d2axissegmentcolor.md) |  |
| [`D2AxisSegmentColorRGB`](d2axissegmentcolorrgb.md) |  |
| [`D2AxisSegmentOrientation`](d2axissegmentorientation.md) |  |
| [`D2AxisSegmentsNo`](d2axissegmentsno.md) |  |
| [`D2AxisSegmentTransparency`](d2axissegmenttransparency.md) |  |
| [`D2AxisSizeInScal`](d2axissizeinscal.md) |  |
| [`D2AxisSyncGrid`](d2axissyncgrid.md) |  |
| [`D2AxisSystem`](d2axissystem.md) |  |
| [`D2AxisTop`](d2axistop.md) |  |
| [`D2AxisXAng`](d2axisxang.md) |  |
| [`D2AxisXAutoColor`](d2axisxautocolor.md) |  |
| [`D2AxisXBegin`](d2axisxbegin.md) |  |
| [`D2AxisXBold`](d2axisxbold.md) |  |
| [`D2AxisXColor`](d2axisxcolor.md) | Valid names: D2AxisXColor, AXCo |
| [`D2AxisXColorRGB`](d2axisxcolorrgb.md) |  |
| [`D2AxisXDivMode`](d2axisxdivmode.md) | Valid names: D2AxisXDivMode, D2AxisXDivModeN |
| [`D2AxisXEnd`](d2axisxend.md) |  |
| [`D2AxisXFont`](d2axisxfont.md) | Valid names: D2AxisXFont, AXFnt |
| [`D2AxisXFormat`](d2axisxformat.md) |  |
| [`D2AxisXFrame`](d2axisxframe.md) |  |
| [`D2AxisXInScal`](d2axisxinscal.md) |  |
| [`D2AxisXItal`](d2axisxital.md) |  |
| [`D2AxisXLineAutoC`](d2axisxlineautoc.md) |  |
| [`D2AxisXLineColor`](d2axisxlinecolor.md) |  |
| [`D2AxisXLineCoRGB`](d2axisxlinecorgb.md) |  |
| [`D2AxisXLineWidth`](d2axisxlinewidth.md) |  |
| [`D2AxisXMiniTick`](d2axisxminitick.md) |  |
| [`D2AxisXNam`](d2axisxnam.md) |  |
| [`D2AxisXNoCurClip`](d2axisxnocurclip.md) |  |
| [`D2AxisXObj`](d2axisxobj.md) |  |
| [`D2AxisXOffOrigin`](d2axisxofforigin.md) |  |
| [`D2AxisXOffset`](d2axisxoffset.md) |  |
| [`D2AxisXOrigin`](d2axisxorigin.md) |  |
| [`D2AxisXRelPos`](d2axisxrelpos.md) |  |
| [`D2AxisXScaleType`](d2axisxscaletype.md) | Valid names: D2AxisXScaleType, D2AxisXScaleTScl, D2AxisXAutoScal |
| [`D2AxisXSize`](d2axisxsize.md) | Valid names: D2AxisXSize; AXSz |
| [`D2AxisXSpanWidth`](d2axisxspanwidth.md) |  |
| [`D2AxisXStrOut`](d2axisxstrout.md) |  |
| [`D2AxisXTick`](d2axisxtick.md) |  |
| [`D2AxisXTickAuto`](d2axisxtickauto.md) |  |
| [`D2AxisXTickBegin`](d2axisxtickbegin.md) |  |
| [`D2AxisXTickChn`](d2axisxtickchn.md) |  |
| [`D2AxisXTickChnN`](d2axisxtickchnn.md) |  |
| [`D2AxisXTickDist`](d2axisxtickdist.md) |  |
| [`D2AxisXTickSize`](d2axisxticksize.md) |  |
| [`D2AxisXTickType`](d2axisxticktype.md) |  |
| [`D2AxisXTxt`](d2axisxtxt.md) |  |
| [`D2AxisXTxtAng`](d2axisxtxtang.md) |  |
| [`D2AxisXTxtAutoCo`](d2axisxtxtautoco.md) |  |
| [`D2AxisXTxtBold`](d2axisxtxtbold.md) | Valid names: D2AxisXTxtBold, ATXB |
| [`D2AxisXTxtColor`](d2axisxtxtcolor.md) | Valid names: D2AxisXTxtColor, ATXCo |
| [`D2AxisXTxtColRGB`](d2axisxtxtcolrgb.md) |  |
| [`D2AxisXTxtDeltaX`](d2axisxtxtdeltax.md) |  |
| [`D2AxisXTxtDeltaY`](d2axisxtxtdeltay.md) |  |
| [`D2AxisXTxtFont`](d2axisxtxtfont.md) | Valid names: D2AxisXTxtFont, ATXFnt |
| [`D2AxisXTxtFrame`](d2axisxtxtframe.md) | Valid names: D2AxisXTxtFrame, ATXF |
| [`D2AxisXTxtItal`](d2axisxtxtital.md) | Valid names: D2AxisXTxtItal, ATXI |
| [`D2AxisXTxtRelPos`](d2axisxtxtrelpos.md) |  |
| [`D2AxisXTxtSize`](d2axisxtxtsize.md) | Valid names: D2AxisXTxtSize, ATXSz |
| [`D2AxisXTxtStrOut`](d2axisxtxtstrout.md) | Valid names: D2AxisXTxtStrOut, ATXO |
| [`D2AxisXTxtUndl`](d2axisxtxtundl.md) | Valid names: D2AxisXTxtUndl, ATXU |
| [`D2AxisXUndl`](d2axisxundl.md) |  |
| [`D2AxisXUnitAuto`](d2axisxunitauto.md) |  |
| [`D2AxisXUnitPerCm`](d2axisxunitpercm.md) | Valid names: D2AxisXUnitPerCm, D2AxisXUnitPUnit |
| [`D2AxisXUnitPreset`](d2axisxunitpreset.md) |  |
| [`D2AxisYAng`](d2axisyang.md) |  |
| [`D2AxisYAutoColor`](d2axisyautocolor.md) |  |
| [`D2AxisYBegin`](d2axisybegin.md) |  |
| [`D2AxisYBold`](d2axisybold.md) |  |
| [`D2AxisYColor`](d2axisycolor.md) | Valid names: D2AxisYColor, AYCo |
| [`D2AxisYColorRGB`](d2axisycolorrgb.md) |  |
| [`D2AxisYDivMode`](d2axisydivmode.md) | Valid names: D2AxisYDivMode, D2AxisYDivModeN, D2AxisYDivModRed |
| [`D2AxisYEnd`](d2axisyend.md) |  |
| [`D2AxisYFont`](d2axisyfont.md) | Valid names: D2AxisYFont, AYFnt |
| [`D2AxisYFormat`](d2axisyformat.md) |  |
| [`D2AxisYFrame`](d2axisyframe.md) |  |
| [`D2AxisYHeigth`](d2axisyheigth.md) |  |
| [`D2AxisYInScal`](d2axisyinscal.md) |  |
| [`D2AxisYItal`](d2axisyital.md) |  |
| [`D2AxisYLineAutoC`](d2axisylineautoc.md) |  |
| [`D2AxisYLineColor`](d2axisylinecolor.md) |  |
| [`D2AxisYLineCoRGB`](d2axisylinecorgb.md) |  |
| [`D2AxisYLineWidth`](d2axisylinewidth.md) |  |
| [`D2AxisYMiniTick`](d2axisyminitick.md) |  |
| [`D2AxisYNam`](d2axisynam.md) |  |
| [`D2AxisYNoCurClip`](d2axisynocurclip.md) |  |
| [`D2AxisYObj`](d2axisyobj.md) |  |
| [`D2AxisYOffOrigin`](d2axisyofforigin.md) |  |
| [`D2AxisYOffset`](d2axisyoffset.md) |  |
| [`D2AxisYOrigin`](d2axisyorigin.md) |  |
| [`D2AxisYRelPos`](d2axisyrelpos.md) |  |
| [`D2AxisYScaleType`](d2axisyscaletype.md) | Valid names: D2AxisYScaleType, D2AxisYScaleTScl, D2AxisYAutoScal |
| [`D2AxisYSize`](d2axisysize.md) | Valid names: D2AxisYSize, AYSz |
| [`D2AxisYSpanWidth`](d2axisyspanwidth.md) |  |
| [`D2AxisYStrOut`](d2axisystrout.md) |  |
| [`D2AxisYTick`](d2axisytick.md) |  |
| [`D2AxisYTickAuto`](d2axisytickauto.md) |  |
| [`D2AxisYTickBegin`](d2axisytickbegin.md) |  |
| [`D2AxisYTickChn`](d2axisytickchn.md) |  |
| [`D2AxisYTickChnN`](d2axisytickchnn.md) |  |
| [`D2AxisYTickDist`](d2axisytickdist.md) |  |
| [`D2AxisYTickSize`](d2axisyticksize.md) |  |
| [`D2AxisYTickType`](d2axisyticktype.md) |  |
| [`D2AxisYTxt`](d2axisytxt.md) |  |
| [`D2AxisYTxtAng`](d2axisytxtang.md) |  |
| [`D2AxisYTxtAutoCo`](d2axisytxtautoco.md) |  |
| [`D2AxisYTxtBold`](d2axisytxtbold.md) | Valid names: D2AxisYTxtBold, ATYB |
| [`D2AxisYTxtColor`](d2axisytxtcolor.md) | Valid names: D2AxisYTxtColor, ATYCo |
| [`D2AxisYTxtColRGB`](d2axisytxtcolrgb.md) |  |
| [`D2AxisYTxtDeltaX`](d2axisytxtdeltax.md) |  |
| [`D2AxisYTxtDeltaY`](d2axisytxtdeltay.md) |  |
| [`D2AxisYTxtFont`](d2axisytxtfont.md) | Valid names: D2AxisYTxtFont, ATYFnt |
| [`D2AxisYTxtFrame`](d2axisytxtframe.md) | Valid names: D2AxisYTxtFrame, ATYF |
| [`D2AxisYTxtItal`](d2axisytxtital.md) | Valid names: D2AxisYTxtItal, ATYI |
| [`D2AxisYTxtRelPos`](d2axisytxtrelpos.md) |  |
| [`D2AxisYTxtSize`](d2axisytxtsize.md) | Valid names: D2AxisYTxtSize, ATYSz |
| [`D2AxisYTxtStrOut`](d2axisytxtstrout.md) | Valid names: D2AxisYTxtStrOut, ATYO |
| [`D2AxisYTxtUndl`](d2axisytxtundl.md) | Valid names: D2AxisYTxtUndl, ATYU |
| [`D2AxisYUndl`](d2axisyundl.md) |  |
| [`D2AxisYUnitAuto`](d2axisyunitauto.md) |  |
| [`D2AxisYUnitPerCm`](d2axisyunitpercm.md) | Valid names: D2AxisYUnitPerCm, D2AxisYUnitPUnit |
| [`D2AxisYUnitPreset`](d2axisyunitpreset.md) |  |
| [`D2BackImageFileName`](d2backimagefilename.md) |  |
| [`D2BackImageFullPath`](d2backimagefullpath.md) |  |
| [`D2BackImageScalingEnable`](d2backimagescalingenable.md) |  |
| [`D2BackImageScalingXBegin`](d2backimagescalingxbegin.md) |  |
| [`D2BackImageScalingXEnd`](d2backimagescalingxend.md) |  |
| [`D2BackImageScalingXUnit`](d2backimagescalingxunit.md) |  |
| [`D2BackImageScalingYBegin`](d2backimagescalingybegin.md) |  |
| [`D2BackImageScalingYEnd`](d2backimagescalingyend.md) |  |
| [`D2BackImageScalingYUnit`](d2backimagescalingyunit.md) |  |
| [`D2CAxisPairNo`](d2caxispairno.md) |  |
| [`D2CChnExpand`](d2cchnexpand.md) |  |
| [`D2CChnX`](d2cchnx.md) |  |
| [`D2CChnXName`](d2cchnxname.md) |  |
| [`D2CChnY`](d2cchny.md) |  |
| [`D2CChnY1`](d2cchny1.md) |  |
| [`D2CChnY1Name`](d2cchny1name.md) |  |
| [`D2CChnYName`](d2cchnyname.md) |  |
| [`D2CConstX`](d2cconstx.md) | Valid names: D2CConstX, D2CCoordinateX |
| [`D2CConstXName`](d2cconstxname.md) | Valid names: D2CConstXName, D2CCoordinateXName |
| [`D2CConstY`](d2cconsty.md) | Valid names: D2CConstY, D2CCoordinateY |
| [`D2CConstYName`](d2cconstyname.md) | Valid names: D2CConstYName, D2CCoordinateYName |
| [`D2CCurveEnable`](d2ccurveenable.md) |  |
| [`D2CCurveLegDrawT`](d2ccurvelegdrawt.md) | Valid names: D2CCurveLegDrawT, D2CCurveLegDraw |
| [`D2CCurveLegSymbolType`](d2ccurvelegsymboltype.md) |  |
| [`D2CCurveLegTxt`](d2ccurvelegtxt.md) |  |
| [`D2CCurveLegTxtA`](d2ccurvelegtxta.md) |  |
| [`D2CCurveTransf`](d2ccurvetransf.md) |  |
| [`D2CCurveType`](d2ccurvetype.md) |  |
| [`D2ConstCTType`](d2constcttype.md) |  |
| [`D2ConstETPos`](d2constetpos.md) |  |
| [`D2ConstETType`](d2constettype.md) |  |
| [`D2CoordinateBoundingType`](d2coordinateboundingtype.md) |  |
| [`D2CoordinateType`](d2coordinatetype.md) |  |
| [`D2CPolarChnExpan`](d2cpolarchnexpan.md) |  |
| [`D2CPolarChnX`](d2cpolarchnx.md) |  |
| [`D2CPolarChnXName`](d2cpolarchnxname.md) |  |
| [`D2CPolarChnY`](d2cpolarchny.md) |  |
| [`D2CPolarChnY1`](d2cpolarchny1.md) |  |
| [`D2CPolarChnY1Nam`](d2cpolarchny1nam.md) |  |
| [`D2CPolarChnYName`](d2cpolarchnyname.md) |  |
| [`D2CPolarCurveTyp`](d2cpolarcurvetyp.md) |  |
| [`D2CPolCrvLegDrwT`](d2cpolcrvlegdrwt.md) | Valid names: D2CPolCrvLegDrwT, D2CPolCrvLegDraw |
| [`D2CPolCrvLegTxt`](d2cpolcrvlegtxt.md) |  |
| [`D2CPolCrvLegTxtA`](d2cpolcrvlegtxta.md) |  |
| [`D2CurSymCFormat`](d2cursymcformat.md) |  |
| [`D2CurSymChn`](d2cursymchn.md) |  |
| [`D2CurSymChnName`](d2cursymchnname.md) |  |
| [`D2CurSymIdxChn`](d2cursymidxchn.md) |  |
| [`D2CurSymIdxCName`](d2cursymidxcname.md) |  |
| [`D2CurSymPFormat`](d2cursympformat.md) |  |
| [`D2CurSymXFormat`](d2cursymxformat.md) |  |
| [`D2CurSymYFormat`](d2cursymyformat.md) | Valid names: D2CurSymYFormat, D2CurveSymFormat |
| [`D2CurveArrowLnColor`](d2curvearrowlncolor.md) |  |
| [`D2CurveArrowLnColRGB`](d2curvearrowlncolrgb.md) |  |
| [`D2CurveArrowLnType`](d2curvearrowlntype.md) |  |
| [`D2CurveArrowLnWidth`](d2curvearrowlnwidth.md) |  |
| [`D2CurveArrowSymbBeg`](d2curvearrowsymbbeg.md) |  |
| [`D2CurveArrowSymbEnd`](d2curvearrowsymbend.md) |  |
| [`D2CurveColor`](d2curvecolor.md) |  |
| [`D2CurveColorRGB`](d2curvecolorrgb.md) |  |
| [`D2CurveCommentVisible`](d2curvecommentvisible.md) |  |
| [`D2CurveDiffType`](d2curvedifftype.md) |  |
| [`D2CurveEbAbsVal`](d2curveebabsval.md) |  |
| [`D2CurveEbColAuto`](d2curveebcolauto.md) |  |
| [`D2CurveEbColor`](d2curveebcolor.md) |  |
| [`D2CurveEbColoRGB`](d2curveebcolorgb.md) |  |
| [`D2CurveEbDispTyp`](d2curveebdisptyp.md) |  |
| [`D2CurveEbError`](d2curveeberror.md) |  |
| [`D2CurveEbLWidth`](d2curveeblwidth.md) |  |
| [`D2CurveEbNegCNam`](d2curveebnegcnam.md) |  |
| [`D2CurveEbNegCNo`](d2curveebnegcno.md) |  |
| [`D2CurveEbPercVal`](d2curveebpercval.md) |  |
| [`D2CurveEbPosCNam`](d2curveebposcnam.md) |  |
| [`D2CurveEbPosCNo`](d2curveebposcno.md) |  |
| [`D2CurveEbType`](d2curveebtype.md) |  |
| [`D2CurveEnable`](d2curveenable.md) |  |
| [`D2CurveETAngle`](d2curveetangle.md) |  |
| [`D2CurveETBackColor`](d2curveetbackcolor.md) |  |
| [`D2CurveETBackColorRGB`](d2curveetbackcolorrgb.md) |  |
| [`D2CurveETBold`](d2curveetbold.md) |  |
| [`D2CurveETColAuto`](d2curveetcolauto.md) |  |
| [`D2CurveETColor`](d2curveetcolor.md) | Valid names: D2CurveETColor, CETCo |
| [`D2CurveETColRGB`](d2curveetcolrgb.md) |  |
| [`D2CurveETFirst`](d2curveetfirst.md) |  |
| [`D2CurveETFont`](d2curveetfont.md) | Valid names: D2CurveETFont, CETFnt |
| [`D2CurveETFrame`](d2curveetframe.md) |  |
| [`D2CurveETItal`](d2curveetital.md) |  |
| [`D2CurveETNV`](d2curveetnv.md) |  |
| [`D2CurveETPos`](d2curveetpos.md) |  |
| [`D2CurveETPosXC`](d2curveetposxc.md) |  |
| [`D2CurveETPosYC`](d2curveetposyc.md) |  |
| [`D2CurveETRelPos`](d2curveetrelpos.md) |  |
| [`D2CurveETShiftX`](d2curveetshiftx.md) |  |
| [`D2CurveETShiftY`](d2curveetshifty.md) |  |
| [`D2CurveETSize`](d2curveetsize.md) | Valid names: D2CurveETSize, CETSz |
| [`D2CurveETStrOut`](d2curveetstrout.md) |  |
| [`D2CurveETTxt`](d2curveettxt.md) |  |
| [`D2CurveETType`](d2curveettype.md) |  |
| [`D2CurveETUndl`](d2curveetundl.md) |  |
| [`D2CurveFillColor`](d2curvefillcolor.md) |  |
| [`D2CurveFillColorMode`](d2curvefillcolormode.md) |  |
| [`D2CurveFillColorRGB`](d2curvefillcolorrgb.md) |  |
| [`D2CurveFillColorRGB2`](d2curvefillcolorrgb2.md) |  |
| [`D2CurveFillMode`](d2curvefillmode.md) |  |
| [`D2CurveFillPattern`](d2curvefillpattern.md) |  |
| [`D2CurveFillPatternType`](d2curvefillpatterntype.md) |  |
| [`D2CurveFillTransparency`](d2curvefilltransparency.md) |  |
| [`D2CurveFillVariant`](d2curvefillvariant.md) |  |
| [`D2CurveFrameBackFMode`](d2curveframebackfmode.md) |  |
| [`D2CurveFrameBackFVariant`](d2curveframebackfvariant.md) |  |
| [`D2CurveFrameBkColor`](d2curveframebkcolor.md) |  |
| [`D2CurveFrameBkColRGB`](d2curveframebkcolrgb.md) |  |
| [`D2CurveFrameBkColRGB2`](d2curveframebkcolrgb2.md) |  |
| [`D2CurveFrameDeltaX`](d2curveframedeltax.md) |  |
| [`D2CurveFrameDeltaY`](d2curveframedeltay.md) |  |
| [`D2CurveFrameHeight`](d2curveframeheight.md) |  |
| [`D2CurveFrameLnColor`](d2curveframelncolor.md) |  |
| [`D2CurveFrameLnColRGB`](d2curveframelncolrgb.md) |  |
| [`D2CurveFrameLnType`](d2curveframelntype.md) |  |
| [`D2CurveFrameLnWidth`](d2curveframelnwidth.md) |  |
| [`D2CurveFrameWidth`](d2curveframewidth.md) |  |
| [`D2CurveHaColor`](d2curvehacolor.md) |  |
| [`D2CurveHaColorAuto`](d2curvehacolorauto.md) |  |
| [`D2CurveHaColRGB`](d2curvehacolrgb.md) |  |
| [`D2CurveHaNo`](d2curvehano.md) |  |
| [`D2CurveHaType`](d2curvehatype.md) |  |
| [`D2CurveHaWidth`](d2curvehawidth.md) |  |
| [`D2CurveInterv`](d2curveinterv.md) |  |
| [`D2CurveLegSymbolType`](d2curvelegsymboltype.md) |  |
| [`D2CurveLineType`](d2curvelinetype.md) |  |
| [`D2CurveLineWidth`](d2curvelinewidth.md) |  |
| [`D2CurveMarkBType`](d2curvemarkbtype.md) |  |
| [`D2CurveMarkColor`](d2curvemarkcolor.md) |  |
| [`D2CurveMarkCoRGB`](d2curvemarkcorgb.md) |  |
| [`D2CurveMarkEType`](d2curvemarketype.md) |  |
| [`D2CurveMarkFColo`](d2curvemarkfcolo.md) |  |
| [`D2CurveMarkFCRGB`](d2curvemarkfcrgb.md) |  |
| [`D2CurveMarkLWidt`](d2curvemarklwidt.md) |  |
| [`D2CurveMarkNType`](d2curvemarkntype.md) |  |
| [`D2CurveMarkRMode`](d2curvemarkrmode.md) |  |
| [`D2CurveMarkRType`](d2curvemarkrtype.md) |  |
| [`D2CurveMarkSize`](d2curvemarksize.md) |  |
| [`D2CurveMarkType`](d2curvemarktype.md) |  |
| [`D2CurveMColAuto`](d2curvemcolauto.md) |  |
| [`D2CurveMFColAuto`](d2curvemfcolauto.md) |  |
| [`D2CurveNovConnec`](d2curvenovconnec.md) |  |
| [`D2CurveObj`](d2curveobj.md) |  |
| [`D2CurvePalColor`](d2curvepalcolor.md) |  |
| [`D2CurvePalColRGB`](d2curvepalcolrgb.md) |  |
| [`D2CurvePalLimit`](d2curvepallimit.md) |  |
| [`D2CurvePalLine`](d2curvepalline.md) |  |
| [`D2CurvePalLType`](d2curvepalltype.md) |  |
| [`D2CurvePalNo`](d2curvepalno.md) |  |
| [`D2CurvePalType`](d2curvepaltype.md) |  |
| [`D2CurvePalValBeg`](d2curvepalvalbeg.md) |  |
| [`D2CurvePalValEnd`](d2curvepalvalend.md) |  |
| [`D2CurvePalWidth`](d2curvepalwidth.md) |  |
| [`D2CurveSmooth`](d2curvesmooth.md) |  |
| [`D2CurveSpColAuto`](d2curvespcolauto.md) |  |
| [`D2CurveSpecColor`](d2curvespeccolor.md) |  |
| [`D2CurveSpecCoRGB`](d2curvespeccorgb.md) |  |
| [`D2CurveSpecInter`](d2curvespecinter.md) |  |
| [`D2CurveSpecLine`](d2curvespecline.md) |  |
| [`D2CurveSpecLWidt`](d2curvespeclwidt.md) |  |
| [`D2CurveSpecOffs`](d2curvespecoffs.md) |  |
| [`D2CurveSpecType`](d2curvespectype.md) |  |
| [`D2CurveSpecWidth`](d2curvespecwidth.md) |  |
| [`D2CurveStairType`](d2curvestairtype.md) |  |
| [`D2CurveSyColAuto`](d2curvesycolauto.md) |  |
| [`D2CurveSymAng`](d2curvesymang.md) |  |
| [`D2CurveSymBackColor`](d2curvesymbackcolor.md) |  |
| [`D2CurveSymBackColorRGB`](d2curvesymbackcolorrgb.md) |  |
| [`D2CurveSymBold`](d2curvesymbold.md) |  |
| [`D2CurveSymBType`](d2curvesymbtype.md) |  |
| [`D2CurveSymCKey`](d2curvesymckey.md) |  |
| [`D2CurveSymColor`](d2curvesymcolor.md) | Valid names: D2CurveSymColor, CSCo |
| [`D2CurveSymColRGB`](d2curvesymcolrgb.md) |  |
| [`D2CurveSymEType`](d2curvesymetype.md) |  |
| [`D2CurveSymFirst`](d2curvesymfirst.md) |  |
| [`D2CurveSymFKey`](d2curvesymfkey.md) |  |
| [`D2CurveSymFont`](d2curvesymfont.md) | Valid names: D2CurveSymFont, CSFnt |
| [`D2CurveSymFrame`](d2curvesymframe.md) |  |
| [`D2CurveSymItal`](d2curvesymital.md) |  |
| [`D2CurveSymNKey`](d2curvesymnkey.md) |  |
| [`D2CurveSymPKey`](d2curvesympkey.md) |  |
| [`D2CurveSymPosTyp`](d2curvesympostyp.md) |  |
| [`D2CurveSymRelPos`](d2curvesymrelpos.md) |  |
| [`D2CurveSymRMode`](d2curvesymrmode.md) |  |
| [`D2CurveSymRType`](d2curvesymrtype.md) |  |
| [`D2CurveSymSepar`](d2curvesymsepar.md) |  |
| [`D2CurveSymSize`](d2curvesymsize.md) | Valid names: D2CurveSymSize, CSSz |
| [`D2CurveSymStrOut`](d2curvesymstrout.md) |  |
| [`D2CurveSymType`](d2curvesymtype.md) |  |
| [`D2CurveSymUndl`](d2curvesymundl.md) |  |
| [`D2CurveSymXDelt`](d2curvesymxdelt.md) |  |
| [`D2CurveSymXKey`](d2curvesymxkey.md) |  |
| [`D2CurveSymYDelt`](d2curvesymydelt.md) |  |
| [`D2CurveSymYKey`](d2curvesymykey.md) |  |
| [`D2CurveTag`](d2curvetag.md) |  |
| [`D2CurveTxt`](d2curvetxt.md) |  |
| [`D2CurveTxtAlignment`](d2curvetxtalignment.md) |  |
| [`D2CurveTxtBold`](d2curvetxtbold.md) |  |
| [`D2CurveTxtColor`](d2curvetxtcolor.md) |  |
| [`D2CurveTxtColorRGB`](d2curvetxtcolorrgb.md) |  |
| [`D2CurveTxtFont`](d2curvetxtfont.md) |  |
| [`D2CurveTxtItal`](d2curvetxtital.md) |  |
| [`D2CurveTxtSize`](d2curvetxtsize.md) |  |
| [`D2CurveTxtStrOut`](d2curvetxtstrout.md) |  |
| [`D2CurveTxtUndl`](d2curvetxtundl.md) |  |
| [`D2CurveType`](d2curvetype.md) |  |
| [`D2GridLineWidth`](d2gridlinewidth.md) |  |
| [`D2HdClip`](d2hdclip.md) |  |
| [`D2HdPropType`](d2hdproptype.md) |  |
| [`D2HdTxtAng`](d2hdtxtang.md) |  |
| [`D2HdTxtBold`](d2hdtxtbold.md) |  |
| [`D2HDTxtCOLOR`](d2hdtxtcolor.md) | Valid names: D2HDTxtCOLOR, D2HdTCo |
| [`D2HdTxtColorRGB`](d2hdtxtcolorrgb.md) |  |
| [`D2HDTxtFONT`](d2hdtxtfont.md) | Valid names: D2HDTxtFONT, D2HdTFnt |
| [`D2HdTxtFrame`](d2hdtxtframe.md) |  |
| [`D2HdTxtItal`](d2hdtxtital.md) |  |
| [`D2HdTxtRelPos`](d2hdtxtrelpos.md) |  |
| [`D2HDTxtSIZE`](d2hdtxtsize.md) | Valid names: D2HDTxtSIZE, D2HdTSz |
| [`D2HdTxtStrOut`](d2hdtxtstrout.md) |  |
| [`D2HdTxtUndl`](d2hdtxtundl.md) |  |
| [`D2HdWordWrap`](d2hdwordwrap.md) |  |
| [`D2LegAngle`](d2legangle.md) |  |
| [`D2LegBackColor`](d2legbackcolor.md) |  |
| [`D2LegBackFMode`](d2legbackfmode.md) |  |
| [`D2LegBackFVariant`](d2legbackfvariant.md) |  |
| [`D2LegBackRGB`](d2legbackrgb.md) |  |
| [`D2LegBackRGB2`](d2legbackrgb2.md) |  |
| [`D2LegClip`](d2legclip.md) |  |
| [`D2LegDraw`](d2legdraw.md) |  |
| [`D2LegFirstOnly`](d2legfirstonly.md) |  |
| [`D2LegFrame`](d2legframe.md) |  |
| [`D2LegFrameCol`](d2legframecol.md) |  |
| [`D2LegFrameColRGB`](d2legframecolrgb.md) |  |
| [`D2LegFrameWidth`](d2legframewidth.md) |  |
| [`D2LegGridLines`](d2leggridlines.md) |  |
| [`D2LegMove`](d2legmove.md) |  |
| [`D2LegNo`](d2legno.md) |  |
| [`D2LegOrient`](d2legorient.md) |  |
| [`D2LegPAngle`](d2legpangle.md) |  |
| [`D2LegPBackColor`](d2legpbackcolor.md) |  |
| [`D2LegPBackFMode`](d2legpbackfmode.md) |  |
| [`D2LegPBackFVariant`](d2legpbackfvariant.md) |  |
| [`D2LegPBackRGB`](d2legpbackrgb.md) |  |
| [`D2LegPBackRGB2`](d2legpbackrgb2.md) |  |
| [`D2LegPClip`](d2legpclip.md) |  |
| [`D2LegPDraw`](d2legpdraw.md) |  |
| [`D2LegPFrame`](d2legpframe.md) |  |
| [`D2LegPFrameCol`](d2legpframecol.md) |  |
| [`D2LegPFrameCRGB`](d2legpframecrgb.md) |  |
| [`D2LegPFrameWidth`](d2legpframewidth.md) |  |
| [`D2LegPMove`](d2legpmove.md) |  |
| [`D2LegPOrient`](d2legporient.md) |  |
| [`D2LegPositionType`](d2legpositiontype.md) |  |
| [`D2LegPosSysRelatedX`](d2legpossysrelatedx.md) |  |
| [`D2LegPosSysRelatedY`](d2legpossysrelatedy.md) |  |
| [`D2LegPosX`](d2legposx.md) |  |
| [`D2LegPosY`](d2legposy.md) |  |
| [`D2LegPPositionType`](d2legppositiontype.md) |  |
| [`D2LegPPosSysRelatedX`](d2legppossysrelatedx.md) |  |
| [`D2LegPPosSysRelatedY`](d2legppossysrelatedy.md) |  |
| [`D2LegPPosX`](d2legpposx.md) |  |
| [`D2LegPPosY`](d2legpposy.md) |  |
| [`D2LegPRelPos`](d2legprelpos.md) |  |
| [`D2LegPSclDomain`](d2legpscldomain.md) |  |
| [`D2LegPSclFormat`](d2legpsclformat.md) |  |
| [`D2LegPSclRed`](d2legpsclred.md) |  |
| [`D2LegPSclType`](d2legpscltype.md) |  |
| [`D2LegPSclValType`](d2legpsclvaltype.md) |  |
| [`D2LegPSizeGlX`](d2legpsizeglx.md) |  |
| [`D2LegPSizeGlY`](d2legpsizegly.md) |  |
| [`D2LegPSizeLoX`](d2legpsizelox.md) |  |
| [`D2LegPSizeLoY`](d2legpsizeloy.md) |  |
| [`D2LegPSizeType`](d2legpsizetype.md) |  |
| [`D2LegPSymDist`](d2legpsymdist.md) |  |
| [`D2LegPSymFrame`](d2legpsymframe.md) |  |
| [`D2LegPSymSize`](d2legpsymsize.md) |  |
| [`D2LegPSymType`](d2legpsymtype.md) |  |
| [`D2LegPTAngle`](d2legptangle.md) |  |
| [`D2LegPTFrame`](d2legptframe.md) |  |
| [`D2LegPTitle`](d2legptitle.md) |  |
| [`D2LegPTRelPos`](d2legptrelpos.md) |  |
| [`D2LegPTSize`](d2legptsize.md) |  |
| [`D2LegPTTxtBold`](d2legpttxtbold.md) | Valid names: D2LegPTTxtBold, D2LPTTB |
| [`D2LegPTTxtCol`](d2legpttxtcol.md) | Valid names: D2LegPTTxtCol, D2LPTTC |
| [`D2LegPTTxtColRGB`](d2legpttxtcolrgb.md) |  |
| [`D2LegPTTxtFont`](d2legpttxtfont.md) | Valid names: D2LegPTTxtFont, D2LPTTF |
| [`D2LegPTTxtFrame`](d2legpttxtframe.md) |  |
| [`D2LegPTTxtItal`](d2legpttxtital.md) | Valid names: D2LegPTTxtItal, D2LPTTI |
| [`D2LegPTTxtSize`](d2legpttxtsize.md) | Valid names: D2LegPTTxtSize, D2LPTTSz |
| [`D2LegPTTxtStrOut`](d2legpttxtstrout.md) | Valid names: D2LegPTTxtStrOut, D2LPTTSO |
| [`D2LegPTTxtSzAut`](d2legpttxtszaut.md) |  |
| [`D2LegPTTxtUndl`](d2legpttxtundl.md) | Valid names: D2LegPTTxtUndl, D2LPTTU |
| [`D2LegPTxtBold`](d2legptxtbold.md) | Valid names: D2LegPTxtBold, D2LPTB |
| [`D2LegPTxtCol`](d2legptxtcol.md) | Valid names: D2LegPTxtCol, D2LPTC |
| [`D2LegPTxtColAut`](d2legptxtcolaut.md) |  |
| [`D2LegPTxtColRGB`](d2legptxtcolrgb.md) |  |
| [`D2LegPTxtFont`](d2legptxtfont.md) | Valid names: D2LegPTxtFont, D2LPTF |
| [`D2LegPTxtItal`](d2legptxtital.md) | Valid names: D2LegPTxtItal, D2LPTI |
| [`D2LegPTxtPos`](d2legptxtpos.md) |  |
| [`D2LegPTxtSize`](d2legptxtsize.md) | Valid names: D2LegPTxtSize, D2LPTSz |
| [`D2LegPTxtSizeAut`](d2legptxtsizeaut.md) |  |
| [`D2LegPTxtStrOut`](d2legptxtstrout.md) | Valid names: D2LegPTxtStrOut, D2LPTSO |
| [`D2LegPTxtUndl`](d2legptxtundl.md) | Valid names: D2LegPTxtUndl, D2LPTU |
| [`D2LegRelPos`](d2legrelpos.md) |  |
| [`D2LegSizeGlX`](d2legsizeglx.md) |  |
| [`D2LegSizeGlY`](d2legsizegly.md) |  |
| [`D2LegSizeLoX`](d2legsizelox.md) |  |
| [`D2LegSizeLoY`](d2legsizeloy.md) |  |
| [`D2LegSizeType`](d2legsizetype.md) |  |
| [`D2LegSymDist`](d2legsymdist.md) |  |
| [`D2LegSymFrame`](d2legsymframe.md) |  |
| [`D2LegSymOrder`](d2legsymorder.md) |  |
| [`D2LegSymSize`](d2legsymsize.md) |  |
| [`D2LegTAngle`](d2legtangle.md) |  |
| [`D2LegTFrame`](d2legtframe.md) |  |
| [`D2LegTitle`](d2legtitle.md) |  |
| [`D2LegTitleA`](d2legtitlea.md) |  |
| [`D2LegTRelPos`](d2legtrelpos.md) |  |
| [`D2LegTSize`](d2legtsize.md) |  |
| [`D2LegTTxtBold`](d2legttxtbold.md) | Valid names: D2LegTTxtBold, D2LTTB |
| [`D2LegTTxtCol`](d2legttxtcol.md) | Valid names: D2LegTTxtCol, D2LTTC |
| [`D2LegTTxtColRGB`](d2legttxtcolrgb.md) |  |
| [`D2LegTTxtFont`](d2legttxtfont.md) | Valid names: D2LegTTxtFont, D2LTTF |
| [`D2LegTTxtFrame`](d2legttxtframe.md) |  |
| [`D2LegTTxtItal`](d2legttxtital.md) | Valid names: D2LegTTxtItal, D2LTTI |
| [`D2LegTTxtSize`](d2legttxtsize.md) | Valid names: D2LegTTxtSize, D2LTTSz |
| [`D2LegTTxtStrOut`](d2legttxtstrout.md) | Valid names: D2LegTTxtStrOut, D2LTTSO |
| [`D2LegTTxtSzAut`](d2legttxtszaut.md) |  |
| [`D2LegTTxtUndl`](d2legttxtundl.md) | Valid names: D2LegTTxtUndl, D2LTTU |
| [`D2LegTxtBold`](d2legtxtbold.md) | Valid names: D2LegTxtBold, D2LTB |
| [`D2LegTxtClip`](d2legtxtclip.md) |  |
| [`D2LegTxtCol`](d2legtxtcol.md) | Valid names: D2LegTxtCol, D2LTC |
| [`D2LegTxtColAut`](d2legtxtcolaut.md) |  |
| [`D2LegTxtColRGB`](d2legtxtcolrgb.md) |  |
| [`D2LegTxtFont`](d2legtxtfont.md) | Valid names: D2LegTxtFont, D2LTF |
| [`D2LegTxtFrame`](d2legtxtframe.md) |  |
| [`D2LegTxtFree`](d2legtxtfree.md) |  |
| [`D2LegTxtFreeA`](d2legtxtfreea.md) |  |
| [`D2LegTxtItal`](d2legtxtital.md) | Valid names: D2LegTxtItal, D2LTI |
| [`D2LegTxtPos`](d2legtxtpos.md) |  |
| [`D2LegTxtRelWidth`](d2legtxtrelwidth.md) |  |
| [`D2LegTxtSize`](d2legtxtsize.md) | Valid names: D2LegTxtSize, D2LTSz |
| [`D2LegTxtSizeAut`](d2legtxtsizeaut.md) |  |
| [`D2LegTxtStrOut`](d2legtxtstrout.md) | Valid names: D2LegTxtStrOut, D2LTSO |
| [`D2LegTxtType`](d2legtxttype.md) |  |
| [`D2LegTxtTypeA`](d2legtxttypea.md) |  |
| [`D2LegTxtUndl`](d2legtxtundl.md) | Valid names: D2LegTxtUndl, D2LTU |
| [`D2LegTxtWordWrap`](d2legtxtwordwrap.md) |  |
| [`D2MTickColor`](d2mtickcolor.md) |  |
| [`D2MTickColorRGB`](d2mtickcolorrgb.md) |  |
| [`D2MTickGridDraw`](d2mtickgriddraw.md) |  |
| [`D2MTickLineInter`](d2mticklineinter.md) |  |
| [`D2MTickLineType`](d2mticklinetype.md) |  |
| [`D2MTickLineWidth`](d2mticklinewidth.md) |  |
| [`D2MultipleScal`](d2multiplescal.md) |  |
| [`D2PolarAngDim`](d2polarangdim.md) |  |
| [`D2PolarAutoScal`](d2polarautoscal.md) |  |
| [`D2PolarBackColor`](d2polarbackcolor.md) |  |
| [`D2PolarBackRGB`](d2polarbackrgb.md) |  |
| [`D2PolarBegin`](d2polarbegin.md) |  |
| [`D2PolarBottom`](d2polarbottom.md) |  |
| [`D2PolarClip`](d2polarclip.md) |  |
| [`D2PolarColor`](d2polarcolor.md) |  |
| [`D2PolarColorRGB`](d2polarcolorrgb.md) |  |
| [`D2PolarCurveNoMx`](d2polarcurvenomx.md) |  |
| [`D2PolarCurveObj`](d2polarcurveobj.md) |  |
| [`D2PolarCurveType`](d2polarcurvetype.md) |  |
| [`D2PolarDivType`](d2polardivtype.md) |  |
| [`D2PolarEnd`](d2polarend.md) |  |
| [`D2PolarInterv`](d2polarinterv.md) |  |
| [`D2PolarLblDirec`](d2polarlbldirec.md) |  |
| [`D2PolarLeft`](d2polarleft.md) |  |
| [`D2PolarLineWidth`](d2polarlinewidth.md) |  |
| [`D2PolarMiniSect`](d2polarminisect.md) |  |
| [`D2PolarMiniStart`](d2polarministart.md) |  |
| [`D2PolarMiniTick`](d2polarminitick.md) |  |
| [`D2PolarNumAng`](d2polarnumang.md) |  |
| [`D2PolarNumBold`](d2polarnumbold.md) | Valid names: D2PolarNumBold, PNBo |
| [`D2PolarNumColor`](d2polarnumcolor.md) | Valid names: D2PolarNumColor, PNCo |
| [`D2PolarNumColRGB`](d2polarnumcolrgb.md) |  |
| [`D2PolarNumFont`](d2polarnumfont.md) |  |
| [`D2PolarNumFormat`](d2polarnumformat.md) |  |
| [`D2PolarNumFrame`](d2polarnumframe.md) |  |
| [`D2PolarNumItal`](d2polarnumital.md) | Valid names: D2PolarNumItal, PNIt |
| [`D2PolarNumRelPos`](d2polarnumrelpos.md) |  |
| [`D2PolarNumSize`](d2polarnumsize.md) | Valid names: D2PolarNumSize, PNSi |
| [`D2PolarNumStrOut`](d2polarnumstrout.md) | Valid names: D2PolarNumStrOut, PNSr |
| [`D2PolarNumUndl`](d2polarnumundl.md) | Valid names: D2PolarNumUndl, PNUn |
| [`D2PolarOpenAng`](d2polaropenang.md) |  |
| [`D2PolarOrigin`](d2polarorigin.md) |  |
| [`D2PolarRight`](d2polarright.md) |  |
| [`D2PolarScalAng`](d2polarscalang.md) |  |
| [`D2PolarSect`](d2polarsect.md) |  |
| [`D2PolarStartLbl`](d2polarstartlbl.md) |  |
| [`D2PolarTick`](d2polartick.md) |  |
| [`D2PolarTickChn`](d2polartickchn.md) |  |
| [`D2PolarTickChnN`](d2polartickchnn.md) |  |
| [`D2PolarTickDist`](d2polartickdist.md) |  |
| [`D2PolarTickType`](d2polarticktype.md) |  |
| [`D2PolarTop`](d2polartop.md) |  |
| [`D2PolarTxt`](d2polartxt.md) |  |
| [`D2PolarTxtAng`](d2polartxtang.md) |  |
| [`D2PolarTxtBold`](d2polartxtbold.md) |  |
| [`D2PolarTxtColor`](d2polartxtcolor.md) | Valid names: D2PolarTxtColor, PTCo |
| [`D2PolarTxtColRGB`](d2polartxtcolrgb.md) |  |
| [`D2PolarTxtDeltaX`](d2polartxtdeltax.md) |  |
| [`D2PolarTxtDeltaY`](d2polartxtdeltay.md) |  |
| [`D2PolarTxtFont`](d2polartxtfont.md) | Valid names: D2PolarTxtFont, PTTFnt |
| [`D2PolarTxtFrame`](d2polartxtframe.md) |  |
| [`D2PolarTxtItal`](d2polartxtital.md) |  |
| [`D2PolarTxtSize`](d2polartxtsize.md) | Valid names: D2PolarTxtSize, PTSz |
| [`D2PolarTxtStrOut`](d2polartxtstrout.md) |  |
| [`D2PolarTxtUndl`](d2polartxtundl.md) |  |
| [`D2PolarType`](d2polartype.md) |  |
| [`D2PolarWhereTxt`](d2polarwheretxt.md) |  |
| [`D2PolarZeroAng`](d2polarzeroang.md) |  |
| [`D2PolCrvLegTxt`](d2polcrvlegtxt.md) |  |
| [`D2PolLegAngle`](d2pollegangle.md) |  |
| [`D2PolLegBackCol`](d2pollegbackcol.md) |  |
| [`D2PolLegBackFMode`](d2pollegbackfmode.md) |  |
| [`D2PolLegBackFVariant`](d2pollegbackfvariant.md) |  |
| [`D2PolLegBackRGB`](d2pollegbackrgb.md) |  |
| [`D2PolLegBackRGB2`](d2pollegbackrgb2.md) |  |
| [`D2PolLegClip`](d2pollegclip.md) |  |
| [`D2PolLegDraw`](d2pollegdraw.md) |  |
| [`D2PolLegFrame`](d2pollegframe.md) |  |
| [`D2PolLegFrameCol`](d2pollegframecol.md) |  |
| [`D2PolLegFrColRGB`](d2pollegfrcolrgb.md) |  |
| [`D2PolLegFrstOnly`](d2pollegfrstonly.md) |  |
| [`D2PolLegFrWidth`](d2pollegfrwidth.md) |  |
| [`D2PolLegGridLines`](d2polleggridlines.md) |  |
| [`D2PolLegMove`](d2pollegmove.md) |  |
| [`D2PolLegNo`](d2pollegno.md) |  |
| [`D2PolLegOrient`](d2pollegorient.md) |  |
| [`D2PolLegPositionType`](d2pollegpositiontype.md) |  |
| [`D2PolLegPosSysRelatedX`](d2pollegpossysrelatedx.md) |  |
| [`D2PolLegPosSysRelatedY`](d2pollegpossysrelatedy.md) |  |
| [`D2PolLegPosX`](d2pollegposx.md) |  |
| [`D2PolLegPosY`](d2pollegposy.md) |  |
| [`D2PolLegRelPos`](d2pollegrelpos.md) |  |
| [`D2PolLegSizeGlX`](d2pollegsizeglx.md) |  |
| [`D2PolLegSizeGlY`](d2pollegsizegly.md) |  |
| [`D2PolLegSizeLoX`](d2pollegsizelox.md) |  |
| [`D2PolLegSizeLoY`](d2pollegsizeloy.md) |  |
| [`D2PolLegSizeType`](d2pollegsizetype.md) |  |
| [`D2PolLegSymSize`](d2pollegsymsize.md) |  |
| [`D2PolLegTAngle`](d2pollegtangle.md) |  |
| [`D2PolLegTFrame`](d2pollegtframe.md) |  |
| [`D2PolLegTitle`](d2pollegtitle.md) |  |
| [`D2PolLegTitleA`](d2pollegtitlea.md) |  |
| [`D2PolLegTRelPos`](d2pollegtrelpos.md) |  |
| [`D2PolLegTSize`](d2pollegtsize.md) |  |
| [`D2PolLegTtxtBold`](d2pollegttxtbold.md) | Valid names: D2PolLegTtxtBold, D2PLTTB |
| [`D2PolLegTtxtCol`](d2pollegttxtcol.md) | Valid names: D2PolLegTtxtCol, D2PLTTC |
| [`D2PolLegTtxtFont`](d2pollegttxtfont.md) | Valid names: D2PolLegTtxtFont, D2PLTTF |
| [`D2PolLegTtxtItal`](d2pollegttxtital.md) | Valid names: D2PolLegTtxtItal, D2PLTTI |
| [`D2PolLegTTxtRGB`](d2pollegttxtrgb.md) |  |
| [`D2PolLegTTxtSAut`](d2pollegttxtsaut.md) |  |
| [`D2PolLegTtxtSize`](d2pollegttxtsize.md) | Valid names: D2PolLegTtxtSize, D2PLTTSz |
| [`D2PolLegTtxtSOut`](d2pollegttxtsout.md) | Valid names: D2PolLegTtxtSOut, D2PLTTSO |
| [`D2PolLegTtxtUndl`](d2pollegttxtundl.md) | Valid names: D2PolLegTtxtUndl, D2PLTTU |
| [`D2PolLegTxtBold`](d2pollegtxtbold.md) | Valid names: D2PolLegTxtBold, D2PLTB |
| [`D2PolLegTxtCAut`](d2pollegtxtcaut.md) |  |
| [`D2PolLegTxtClip`](d2pollegtxtclip.md) |  |
| [`D2PolLegTxtCol`](d2pollegtxtcol.md) | Valid names: D2PolLegTxtCol, D2PLTC |
| [`D2PolLegTxtFont`](d2pollegtxtfont.md) | Valid names: D2PolLegTxtFont, D2PLTF |
| [`D2PolLegTxtFree`](d2pollegtxtfree.md) |  |
| [`D2PolLegTxtFreeA`](d2pollegtxtfreea.md) |  |
| [`D2PolLegTxtItal`](d2pollegtxtital.md) | Valid names: D2PolLegTxtItal, D2PLTI |
| [`D2PolLegTxtPos`](d2pollegtxtpos.md) |  |
| [`D2PolLegTxtRelWi`](d2pollegtxtrelwi.md) |  |
| [`D2PolLegTxtRGB`](d2pollegtxtrgb.md) |  |
| [`D2PolLegTxtSAut`](d2pollegtxtsaut.md) |  |
| [`D2PolLegTxtSize`](d2pollegtxtsize.md) | Valid names: D2PolLegTxtSize, D2PLTSz |
| [`D2PolLegTxtSOut`](d2pollegtxtsout.md) | Valid names: D2PolLegTxtSOut, D2PLTSO |
| [`D2PolLegTxtType`](d2pollegtxttype.md) |  |
| [`D2PolLegTxtTypeA`](d2pollegtxttypea.md) |  |
| [`D2PolLegTxtUndl`](d2pollegtxtundl.md) | Valid names: D2PolLegTxtUndl, D2PLTU |
| [`D2PolLegTxtWordWrap`](d2pollegtxtwordwrap.md) |  |
| [`D2SearchMode`](d2searchmode.md) | Specifies a condition. |
| [`D2TabAutoScalTyp`](d2tabautoscaltyp.md) | Valid names: D2TabAutoScalTyp, D2TabAutoScal |
| [`D2TabBackColor`](d2tabbackcolor.md) |  |
| [`D2TabBackFMode`](d2tabbackfmode.md) |  |
| [`D2TabBackFVariant`](d2tabbackfvariant.md) |  |
| [`D2TabBackRGB`](d2tabbackrgb.md) |  |
| [`D2TabBackRGB2`](d2tabbackrgb2.md) |  |
| [`D2TabBegin`](d2tabbegin.md) |  |
| [`D2TabBottom`](d2tabbottom.md) |  |
| [`D2TabChn`](d2tabchn.md) |  |
| [`D2TabChnCountAll`](d2tabchncountall.md) | Receives the total number of all channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnCountVisible`](d2tabchncountvisible.md) | Receives the total number of the visible channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnMaxAll`](d2tabchnmaxall.md) | Receives the maximum value of all channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnMaxAll`](d2tabchnmaxall-2.md) | Receives the arithmetic mean value of all channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnMaxVisible`](d2tabchnmaxvisible.md) | Receives the maximum value of the visible channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnMaxVisible`](d2tabchnmaxvisible-2.md) | Receives the arithmetic mean value of all visible channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnMinAll`](d2tabchnminall.md) | Receives the minimum value of all channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnMinVisible`](d2tabchnminvisible.md) | Receives the minimum value of the visible channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnName`](d2tabchnname.md) |  |
| [`D2TabChnSumAll`](d2tabchnsumall.md) | Receives the sum of all channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabChnSumVisible`](d2tabchnsumvisible.md) | Receives the sum of the visible channel values in a 2D table column. Use this variable in the headers or footers of the 2D table columns. |
| [`D2TabCol`](d2tabcol.md) | Specifies the column index of the 2D table. |
| [`D2TabColHeight`](d2tabcolheight.md) |  |
| [`D2TabDataType`](d2tabdatatype.md) |  |
| [`D2TabDirec`](d2tabdirec.md) |  |
| [`D2TabEnd`](d2tabend.md) |  |
| [`D2TabGrid`](d2tabgrid.md) |  |
| [`D2TabHdClip`](d2tabhdclip.md) |  |
| [`D2TabHdWordWrap`](d2tabhdwordwrap.md) |  |
| [`D2TabHeaderTxt`](d2tabheadertxt.md) |  |
| [`D2TabLeft`](d2tableft.md) |  |
| [`D2TabLineColor`](d2tablinecolor.md) |  |
| [`D2TabLineColorV`](d2tablinecolorv.md) |  |
| [`D2TabLineColRGB`](d2tablinecolrgb.md) |  |
| [`D2TabLineColVRGB`](d2tablinecolvrgb.md) |  |
| [`D2TabLineWidth`](d2tablinewidth.md) |  |
| [`D2TabMaxCurveNo`](d2tabmaxcurveno.md) |  |
| [`D2TabNoDist`](d2tabnodist.md) |  |
| [`D2TabNumAng`](d2tabnumang.md) |  |
| [`D2TabNumAutoScal`](d2tabnumautoscal.md) |  |
| [`D2TabNumBold`](d2tabnumbold.md) | Valid names: D2TabNumBold, TTB |
| [`D2TabNumClip`](d2tabnumclip.md) |  |
| [`D2TabNumColor`](d2tabnumcolor.md) |  |
| [`D2TabNumColorRGB`](d2tabnumcolorrgb.md) |  |
| [`D2TabNumFont`](d2tabnumfont.md) |  |
| [`D2TabNumFormat`](d2tabnumformat.md) |  |
| [`D2TabNumFrame`](d2tabnumframe.md) | Valid names: D2TabNumFrame, TTF |
| [`D2TabNumItalic`](d2tabnumitalic.md) | Valid names: D2TabNumItalic, TTI |
| [`D2TabNumPalColor`](d2tabnumpalcolor.md) |  |
| [`D2TabNumPalCoRGB`](d2tabnumpalcorgb.md) |  |
| [`D2TabNumRelPos`](d2tabnumrelpos.md) |  |
| [`D2TabNumSize`](d2tabnumsize.md) |  |
| [`D2TabNumStrOut`](d2tabnumstrout.md) | Valid names: D2TabNumStrOut, TTS |
| [`D2TabNumUndl`](d2tabnumundl.md) | Valid names: D2TabNumUndl, TTU |
| [`D2TabNumWordWrap`](d2tabnumwordwrap.md) |  |
| [`D2TabOptionalLen`](d2taboptionallen.md) |  |
| [`D2TabRelWidth`](d2tabrelwidth.md) |  |
| [`D2TabRight`](d2tabright.md) |  |
| [`D2TabRow`](d2tabrow.md) | Specifies the row index of the 2D table. |
| [`D2TabRowIndex`](d2tabrowindex.md) | Contains the absolute index of the displayed channel value when tables increase. |
| [`D2TabTextColumn`](d2tabtextcolumn.md) |  |
| [`D2TabTextCount`](d2tabtextcount.md) |  |
| [`D2TabTextList`](d2tabtextlist.md) |  |
| [`D2TabTextListLength`](d2tabtextlistlength.md) |  |
| [`D2TabTextRow`](d2tabtextrow.md) |  |
| [`D2TabTop`](d2tabtop.md) |  |
| [`D2TabTxt`](d2tabtxt.md) |  |
| [`D2TabTxtAng`](d2tabtxtang.md) |  |
| [`D2TabTxtAutoScal`](d2tabtxtautoscal.md) |  |
| [`D2TabTxtBold`](d2tabtxtbold.md) |  |
| [`D2TabTxtColor`](d2tabtxtcolor.md) | Valid names: D2TabTxtColor, TTCo |
| [`D2TabTxtColorRGB`](d2tabtxtcolorrgb.md) |  |
| [`D2TabTxtDrawLine`](d2tabtxtdrawline.md) |  |
| [`D2TabTxtField`](d2tabtxtfield.md) |  |
| [`D2TabTxtFont`](d2tabtxtfont.md) | Valid names: D2TabTxtFont, TTFnt |
| [`D2TabTxtFrame`](d2tabtxtframe.md) |  |
| [`D2TabTxtItal`](d2tabtxtital.md) |  |
| [`D2TabTxtRelPos`](d2tabtxtrelpos.md) |  |
| [`D2TabTxtSize`](d2tabtxtsize.md) | Valid names: D2TabTxtSize, TTSz |
| [`D2TabTxtStrOut`](d2tabtxtstrout.md) |  |
| [`D2TabTxtType`](d2tabtxttype.md) |  |
| [`D2TabTxtUndl`](d2tabtxtundl.md) |  |
| [`D2TabTxtVector`](d2tabtxtvector.md) |  |
| [`D2TabVariable`](d2tabvariable.md) |  |
| [`D2TabXDoubleLine`](d2tabxdoubleline.md) |  |
| [`D2TabYDoubleLine`](d2tabydoubleline.md) |  |
| [`D2UseCommonXChn`](d2usecommonxchn.md) |  |
| [`D3ApprAnsatzCoef`](d3appransatzcoef.md) | Receives the coefficients of the setup functions of the 3D approximation. |
| [`D3ApprAnsatzFct`](d3appransatzfct.md) | Specifies the terms of a setup function in the 3D approximation. |
| [`D3ApprAnsatzName`](d3appransatzname.md) | Receives the name of the selected setup functions for the 3D approximation. |
| [`D3ApprAnsatzNo`](d3appransatzno.md) | Receives the number of selected setup functions for the 3D approximation. |
| [`D3ApprClipCopy`](d3apprclipcopy.md) | Specifies whether DIAdem transfers the coefficients of the setup function of the 3D approximation to the clipboard. |
| [`D3ApprClipType`](d3apprcliptype.md) | Specifies whether DIAdem transfers the formatted setup function or a table of the coefficients to the clipboard when DIAdem runs the 3D-approximation. |
| [`D3ApprClipValue`](d3apprclipvalue.md) | Specifies whether DIAdem transfers the results of the 3D approximation to the clipboard as a value or as a variable reference. |
| [`D3ApprFctStr`](d3apprfctstr.md) | Receives the setup function used by the 3D approximation. |
| [`D3AxisAng`](d3axisang.md) |  |
| [`D3AxisAutoPos`](d3axisautopos.md) |  |
| [`D3AxisAutoScaling`](d3axisautoscaling.md) | Valid names: D3AxisAutoScaling, D3AxisAutoScal |
| [`D3AxisBegin`](d3axisbegin.md) |  |
| [`D3AxisBold`](d3axisbold.md) | Valid names: D3AxisBold, D3ABld |
| [`D3AxisBottom`](d3axisbottom.md) |  |
| [`D3AxisColor`](d3axiscolor.md) | Valid names: D3AxisColor, D3ACo |
| [`D3AxisColorRGB`](d3axiscolorrgb.md) |  |
| [`D3AxisEnableInteractiveRotation`](d3axisenableinteractiverotation.md) |  |
| [`D3AxisEnd`](d3axisend.md) |  |
| [`D3AxisFont`](d3axisfont.md) | Valid names: D3AxisFont, D3AFnt |
| [`D3AxisFormat`](d3axisformat.md) |  |
| [`D3AxisFrame`](d3axisframe.md) |  |
| [`D3AxisIso`](d3axisiso.md) |  |
| [`D3AxisIsoLength`](d3axisisolength.md) |  |
| [`D3AxisItal`](d3axisital.md) | Valid names: D3AxisItal, D3AIt |
| [`D3AxisLColor`](d3axislcolor.md) |  |
| [`D3AxisLColorRGB`](d3axislcolorrgb.md) |  |
| [`D3AxisLeft`](d3axisleft.md) |  |
| [`D3AxisLWidth`](d3axislwidth.md) |  |
| [`D3AxisMiniTick`](d3axisminitick.md) |  |
| [`D3AxisOrigin`](d3axisorigin.md) |  |
| [`D3AxisRelPos`](d3axisrelpos.md) |  |
| [`D3AxisRight`](d3axisright.md) |  |
| [`D3AxisRotateX`](d3axisrotatex.md) |  |
| [`D3AxisRotateZ`](d3axisrotatez.md) |  |
| [`D3AxisSize`](d3axissize.md) | Valid names: D3AxisSize, D3ASz |
| [`D3AxisStrOut`](d3axisstrout.md) | Valid names: D3AxisStrOut, D3ASt |
| [`D3AxisTick`](d3axistick.md) |  |
| [`D3AxisTickChn`](d3axistickchn.md) |  |
| [`D3AxisTickChnNam`](d3axistickchnnam.md) |  |
| [`D3AxisTickType`](d3axisticktype.md) |  |
| [`D3AxisTickTypeX`](d3axisticktypex.md) |  |
| [`D3AxisTickTypeY`](d3axisticktypey.md) |  |
| [`D3AxisTickTypeZ`](d3axisticktypez.md) |  |
| [`D3AxisTop`](d3axistop.md) |  |
| [`D3AxisTxt`](d3axistxt.md) |  |
| [`D3AxisTxtAng`](d3axistxtang.md) |  |
| [`D3AxisTxtAngAuto`](d3axistxtangauto.md) |  |
| [`D3AxisTxtBold`](d3axistxtbold.md) | Valid names: D3AxisTxtBold, D3ATBld |
| [`D3AxisTxtColor`](d3axistxtcolor.md) | Valid names: D3AxisTxtColor, D3ATCo |
| [`D3AxisTxtColRGB`](d3axistxtcolrgb.md) |  |
| [`D3AxisTxtDelta1`](d3axistxtdelta1.md) |  |
| [`D3AxisTxtDelta2`](d3axistxtdelta2.md) |  |
| [`D3AxisTxtFont`](d3axistxtfont.md) | Valid names: D3AxisTxtFont, D3ATFnt |
| [`D3AxisTxtFrame`](d3axistxtframe.md) |  |
| [`D3AxisTxtItal`](d3axistxtital.md) | Valid names: D3AxisTxtItal, D3ATIt |
| [`D3AxisTxtSize`](d3axistxtsize.md) | Valid names: D3AxisTxtSize, D3ATSz |
| [`D3AxisTxtStrOut`](d3axistxtstrout.md) | Valid names: D3AxisTxtStrOut, D3ATSt |
| [`D3AxisTxtUndl`](d3axistxtundl.md) | Valid names: D3AxisTxtUndl, D3ATUnd |
| [`D3AxisType`](d3axistype.md) |  |
| [`D3AxisUndl`](d3axisundl.md) |  |
| [`D3AxisWndWhole`](d3axiswndwhole.md) |  |
| [`D3CChnX`](d3cchnx.md) |  |
| [`D3CChnX1`](d3cchnx1.md) |  |
| [`D3CChnX1Name`](d3cchnx1name.md) |  |
| [`D3CChnXName`](d3cchnxname.md) |  |
| [`D3CChnY`](d3cchny.md) |  |
| [`D3CChnY1`](d3cchny1.md) |  |
| [`D3CChnY1Name`](d3cchny1name.md) |  |
| [`D3CChnYName`](d3cchnyname.md) |  |
| [`D3CChnZ`](d3cchnz.md) |  |
| [`D3CChnZ1`](d3cchnz1.md) |  |
| [`D3CChnZ1Name`](d3cchnz1name.md) |  |
| [`D3CChnZName`](d3cchnzname.md) |  |
| [`D3CConstX`](d3cconstx.md) | Valid names: D3CConstX, D3CCoordinateX |
| [`D3CConstXName`](d3cconstxname.md) | Valid names: D3CConstXName, D3CCoordinateXName |
| [`D3CConstY`](d3cconsty.md) | Valid names: D3CConstY, D3CCoordinateY |
| [`D3CConstYName`](d3cconstyname.md) | Valid names: D3CConstYName, D3CCoordinateYName |
| [`D3CConstZ`](d3cconstz.md) | Valid names: D3CConstZ, D3CCoordinateZ |
| [`D3CConstZName`](d3cconstzname.md) | Valid names: D3CConstZName, D3CCoordinateZName |
| [`D3CCurveCDDiffTy`](d3ccurvecddiffty.md) |  |
| [`D3CCurveCDType`](d3ccurvecdtype.md) |  |
| [`D3CCurveIsoNo`](d3ccurveisono.md) |  |
| [`D3CCurveIsoType`](d3ccurveisotype.md) |  |
| [`D3CCurveIsoVar`](d3ccurveisovar.md) |  |
| [`D3CCurveLegDrawT`](d3ccurvelegdrawt.md) | Valid names: D3CCurveLegDrawT, D3CCurveLegDraw |
| [`D3CCurveLegTxt`](d3ccurvelegtxt.md) |  |
| [`D3CCurveLegTxtA`](d3ccurvelegtxta.md) |  |
| [`D3CCurveStruc`](d3ccurvestruc.md) |  |
| [`D3CCurveStruc1`](d3ccurvestruc1.md) |  |
| [`D3CCurveType`](d3ccurvetype.md) |  |
| [`D3CCurveVPlaneTy`](d3ccurvevplanety.md) |  |
| [`D3CCurveVType`](d3ccurvevtype.md) |  |
| [`D3CheckZValue`](d3checkzvalue.md) | Specifies whether DIAdem checks the z-value. If the z-value lies outside the specified limits, the value is invalid. |
| [`D3ConstCTType`](d3constcttype.md) |  |
| [`D3ConstX`](d3constx.md) | Valid names: D3ConstX, D3CoordinateX |
| [`D3ConstXName`](d3constxname.md) |  |
| [`D3ConstY`](d3consty.md) | Valid names: D3ConstY, D3CoordinateY |
| [`D3ConstYName`](d3constyname.md) |  |
| [`D3ConstZ`](d3constz.md) | Valid names: D3ConstZ, D3CoordinateZ |
| [`D3ConstZName`](d3constzname.md) |  |
| [`D3ConvertMode`](d3convertmode.md) | Specifies the conversion mode for three dimensional data. |
| [`D3ConvertRedMode`](d3convertredmode.md) | Specifies how DIAdem combines three-dimensional data when DIAdem converts a triplet to a matrix. By default the D3ConvertRedMode variable contains the value mean . |
| [`D3ConvertTol`](d3converttol.md) | Specifies the tolerance as a percentage within which DIAdem combines value pairs into single values. |
| [`D3ConvertTolAbsX`](d3converttolabsx.md) | Specifies the absolute tolerance within which DIAdem combines x-values into a single value. |
| [`D3ConvertTolAbsY`](d3converttolabsy.md) | Specifies the absolute tolerance within which DIAdem combines y-values into a single value. |
| [`D3ConvertTolMode`](d3converttolmode.md) | Specifies whether DIAdem checks the similarity of two value pairs using relative or absolute exactness. |
| [`D3CoordinateBoundingType`](d3coordinateboundingtype.md) |  |
| [`D3CoordinateType`](d3coordinatetype.md) |  |
| [`D3CrvAddEnvelope`](d3crvaddenvelope.md) |  |
| [`D3CrvAddEnvPt`](d3crvaddenvpt.md) |  |
| [`D3CrvAddMax`](d3crvaddmax.md) |  |
| [`D3CrvAddMin`](d3crvaddmin.md) |  |
| [`D3CrvAddMPt`](d3crvaddmpt.md) |  |
| [`D3CrvCDAddExtIso`](d3crvcdaddextiso.md) |  |
| [`D3CrvCDAddIso`](d3crvcdaddiso.md) |  |
| [`D3CrvCDAddSurf`](d3crvcdaddsurf.md) |  |
| [`D3CrvCDPartialLoadTolerance`](d3crvcdpartialloadtolerance.md) |  |
| [`D3CrvCDTripletDistribution`](d3crvcdtripletdistribution.md) |  |
| [`D3CrvEnvChn`](d3crvenvchn.md) |  |
| [`D3CrvEnvChnName`](d3crvenvchnname.md) |  |
| [`D3CrvEnvColor`](d3crvenvcolor.md) |  |
| [`D3CrvEnvColorRGB`](d3crvenvcolorrgb.md) |  |
| [`D3CrvEnvExtrapol`](d3crvenvextrapol.md) |  |
| [`D3CrvEnvInterv`](d3crvenvinterv.md) |  |
| [`D3CrvEnvLineType`](d3crvenvlinetype.md) |  |
| [`D3CrvEnvMrkCAuto`](d3crvenvmrkcauto.md) |  |
| [`D3CrvEnvMrkColor`](d3crvenvmrkcolor.md) |  |
| [`D3CrvEnvMrkCRGB`](d3crvenvmrkcrgb.md) |  |
| [`D3CrvEnvMrkFCAut`](d3crvenvmrkfcaut.md) |  |
| [`D3CrvEnvMrkFColo`](d3crvenvmrkfcolo.md) |  |
| [`D3CrvEnvMrkFCRGB`](d3crvenvmrkfcrgb.md) |  |
| [`D3CrvEnvMrkLWidt`](d3crvenvmrklwidt.md) |  |
| [`D3CrvEnvMrkSize`](d3crvenvmrksize.md) |  |
| [`D3CrvEnvMrkType`](d3crvenvmrktype.md) |  |
| [`D3CrvEnvSymAng`](d3crvenvsymang.md) |  |
| [`D3CrvEnvSymBold`](d3crvenvsymbold.md) |  |
| [`D3CrvEnvSymColor`](d3crvenvsymcolor.md) |  |
| [`D3CrvEnvSymCRGB`](d3crvenvsymcrgb.md) |  |
| [`D3CrvEnvSymFmt`](d3crvenvsymfmt.md) |  |
| [`D3CrvEnvSymFont`](d3crvenvsymfont.md) |  |
| [`D3CrvEnvSymFrame`](d3crvenvsymframe.md) |  |
| [`D3CrvEnvSymItal`](d3crvenvsymital.md) |  |
| [`D3CrvEnvSymRPos`](d3crvenvsymrpos.md) |  |
| [`D3CrvEnvSymSize`](d3crvenvsymsize.md) |  |
| [`D3CrvEnvSymSOut`](d3crvenvsymsout.md) |  |
| [`D3CrvEnvSymUndl`](d3crvenvsymundl.md) |  |
| [`D3CrvEnvSymZDraw`](d3crvenvsymzdraw.md) |  |
| [`D3CrvEnvType`](d3crvenvtype.md) |  |
| [`D3CrvEnvWidth`](d3crvenvwidth.md) |  |
| [`D3CrvIsoTxtAng`](d3crvisotxtang.md) |  |
| [`D3CrvIsoTxtBold`](d3crvisotxtbold.md) |  |
| [`D3CrvIsoTxtCAuto`](d3crvisotxtcauto.md) |  |
| [`D3CrvIsoTxtColor`](d3crvisotxtcolor.md) |  |
| [`D3CrvIsoTxtCRGB`](d3crvisotxtcrgb.md) |  |
| [`D3CrvIsoTxtFmt`](d3crvisotxtfmt.md) |  |
| [`D3CrvIsoTxtFont`](d3crvisotxtfont.md) |  |
| [`D3CrvIsoTxtFrame`](d3crvisotxtframe.md) |  |
| [`D3CrvIsoTxtItal`](d3crvisotxtital.md) |  |
| [`D3CrvIsoTxtLabel`](d3crvisotxtlabel.md) |  |
| [`D3CrvIsoTxtNType`](d3crvisotxtntype.md) |  |
| [`D3CrvIsoTxtRMode`](d3crvisotxtrmode.md) |  |
| [`D3CrvIsoTxtRPos`](d3crvisotxtrpos.md) |  |
| [`D3CrvIsoTxtRType`](d3crvisotxtrtype.md) |  |
| [`D3CrvIsoTxtSize`](d3crvisotxtsize.md) |  |
| [`D3CrvIsoTxtSOut`](d3crvisotxtsout.md) |  |
| [`D3CrvIsoTxtUndl`](d3crvisotxtundl.md) |  |
| [`D3CrvMaxMrkCAuto`](d3crvmaxmrkcauto.md) |  |
| [`D3CrvMaxMrkColor`](d3crvmaxmrkcolor.md) |  |
| [`D3CrvMaxMrkCRGB`](d3crvmaxmrkcrgb.md) |  |
| [`D3CrvMaxMrkFCAut`](d3crvmaxmrkfcaut.md) |  |
| [`D3CrvMaxMrkFColo`](d3crvmaxmrkfcolo.md) |  |
| [`D3CrvMaxMrkFCRGB`](d3crvmaxmrkfcrgb.md) |  |
| [`D3CrvMaxMrkLWidt`](d3crvmaxmrklwidt.md) |  |
| [`D3CrvMaxMrkSize`](d3crvmaxmrksize.md) |  |
| [`D3CrvMaxMrkType`](d3crvmaxmrktype.md) |  |
| [`D3CrvMaxSymAng`](d3crvmaxsymang.md) |  |
| [`D3CrvMaxSymBold`](d3crvmaxsymbold.md) |  |
| [`D3CrvMaxSymColor`](d3crvmaxsymcolor.md) |  |
| [`D3CrvMaxSymCRGB`](d3crvmaxsymcrgb.md) |  |
| [`D3CrvMaxSymFmt`](d3crvmaxsymfmt.md) |  |
| [`D3CrvMaxSymFont`](d3crvmaxsymfont.md) |  |
| [`D3CrvMaxSymFrame`](d3crvmaxsymframe.md) |  |
| [`D3CrvMaxSymItal`](d3crvmaxsymital.md) |  |
| [`D3CrvMaxSymRPos`](d3crvmaxsymrpos.md) |  |
| [`D3CrvMaxSymSize`](d3crvmaxsymsize.md) |  |
| [`D3CrvMaxSymSOut`](d3crvmaxsymsout.md) |  |
| [`D3CrvMaxSymUndl`](d3crvmaxsymundl.md) |  |
| [`D3CrvMaxSymZDraw`](d3crvmaxsymzdraw.md) |  |
| [`D3CrvMinMrkCAuto`](d3crvminmrkcauto.md) |  |
| [`D3CrvMinMrkColor`](d3crvminmrkcolor.md) |  |
| [`D3CrvMinMrkCRGB`](d3crvminmrkcrgb.md) |  |
| [`D3CrvMinMrkFCAut`](d3crvminmrkfcaut.md) |  |
| [`D3CrvMinMrkFColo`](d3crvminmrkfcolo.md) |  |
| [`D3CrvMinMrkFCRGB`](d3crvminmrkfcrgb.md) |  |
| [`D3CrvMinMrkLWidt`](d3crvminmrklwidt.md) |  |
| [`D3CrvMinMrkSize`](d3crvminmrksize.md) |  |
| [`D3CrvMinMrkType`](d3crvminmrktype.md) |  |
| [`D3CrvMinSymAng`](d3crvminsymang.md) |  |
| [`D3CrvMinSymBold`](d3crvminsymbold.md) |  |
| [`D3CrvMinSymColor`](d3crvminsymcolor.md) |  |
| [`D3CrvMinSymCRGB`](d3crvminsymcrgb.md) |  |
| [`D3CrvMinSymFmt`](d3crvminsymfmt.md) |  |
| [`D3CrvMinSymFont`](d3crvminsymfont.md) |  |
| [`D3CrvMinSymFrame`](d3crvminsymframe.md) |  |
| [`D3CrvMinSymItal`](d3crvminsymital.md) |  |
| [`D3CrvMinSymRPos`](d3crvminsymrpos.md) |  |
| [`D3CrvMinSymSize`](d3crvminsymsize.md) |  |
| [`D3CrvMinSymSOut`](d3crvminsymsout.md) |  |
| [`D3CrvMinSymUndl`](d3crvminsymundl.md) |  |
| [`D3CrvMinSymZDraw`](d3crvminsymzdraw.md) |  |
| [`D3CrvMPtMrkCAuto`](d3crvmptmrkcauto.md) |  |
| [`D3CrvMPtMrkColor`](d3crvmptmrkcolor.md) |  |
| [`D3CrvMPtMrkCRGB`](d3crvmptmrkcrgb.md) |  |
| [`D3CrvMPtMrkFCAut`](d3crvmptmrkfcaut.md) |  |
| [`D3CrvMPtMrkFColo`](d3crvmptmrkfcolo.md) |  |
| [`D3CrvMPtMrkFCRGB`](d3crvmptmrkfcrgb.md) |  |
| [`D3CrvMPtMrkLWidt`](d3crvmptmrklwidt.md) |  |
| [`D3CrvMPtMrkSize`](d3crvmptmrksize.md) |  |
| [`D3CrvMPtMrkType`](d3crvmptmrktype.md) |  |
| [`D3CrvMPtSymAng`](d3crvmptsymang.md) |  |
| [`D3CrvMPtSymBold`](d3crvmptsymbold.md) |  |
| [`D3CrvMPtSymColor`](d3crvmptsymcolor.md) |  |
| [`D3CrvMPtSymCRGB`](d3crvmptsymcrgb.md) |  |
| [`D3CrvMPtSymFmt`](d3crvmptsymfmt.md) |  |
| [`D3CrvMPtSymFont`](d3crvmptsymfont.md) |  |
| [`D3CrvMPtSymFrame`](d3crvmptsymframe.md) |  |
| [`D3CrvMPtSymItal`](d3crvmptsymital.md) |  |
| [`D3CrvMPtSymRPos`](d3crvmptsymrpos.md) |  |
| [`D3CrvMPtSymSize`](d3crvmptsymsize.md) |  |
| [`D3CrvMPtSymSOut`](d3crvmptsymsout.md) |  |
| [`D3CrvMPtSymUndl`](d3crvmptsymundl.md) |  |
| [`D3CrvMPtSymZDraw`](d3crvmptsymzdraw.md) |  |
| [`D3CurveAddCur`](d3curveaddcur.md) |  |
| [`D3CurveAddIso`](d3curveaddiso.md) |  |
| [`D3CurveAddSpike`](d3curveaddspike.md) |  |
| [`D3CurveAddSym`](d3curveaddsym.md) |  |
| [`D3CurveArrowLnColor`](d3curvearrowlncolor.md) |  |
| [`D3CurveArrowLnColRGB`](d3curvearrowlncolrgb.md) |  |
| [`D3CurveArrowLnType`](d3curvearrowlntype.md) |  |
| [`D3CurveArrowLnWidth`](d3curvearrowlnwidth.md) |  |
| [`D3CurveArrowSymbBeg`](d3curvearrowsymbbeg.md) |  |
| [`D3CurveArrowSymbEnd`](d3curvearrowsymbend.md) |  |
| [`D3CurveCDDiffTy`](d3curvecddiffty.md) |  |
| [`D3CurveCDType`](d3curvecdtype.md) |  |
| [`D3CurveColor`](d3curvecolor.md) |  |
| [`D3CurveColor2`](d3curvecolor2.md) |  |
| [`D3CurveColor2RGB`](d3curvecolor2rgb.md) |  |
| [`D3CurveColorRGB`](d3curvecolorrgb.md) |  |
| [`D3CurveCommentVisible`](d3curvecommentvisible.md) |  |
| [`D3CurveConsiderIsoValForAutoScal`](d3curveconsiderisovalforautoscal.md) |  |
| [`D3CurveETAngle`](d3curveetangle.md) |  |
| [`D3CurveETBackColor`](d3curveetbackcolor.md) |  |
| [`D3CurveETBackColorRGB`](d3curveetbackcolorrgb.md) |  |
| [`D3CurveETBold`](d3curveetbold.md) |  |
| [`D3CurveETColAuto`](d3curveetcolauto.md) |  |
| [`D3CurveETColor`](d3curveetcolor.md) |  |
| [`D3CurveETColRGB`](d3curveetcolrgb.md) |  |
| [`D3CurveETFont`](d3curveetfont.md) |  |
| [`D3CurveETFrame`](d3curveetframe.md) |  |
| [`D3CurveETItal`](d3curveetital.md) |  |
| [`D3CurveETPosXC`](d3curveetposxc.md) |  |
| [`D3CurveETPosYC`](d3curveetposyc.md) |  |
| [`D3CurveETRelPos`](d3curveetrelpos.md) |  |
| [`D3CurveETShiftX`](d3curveetshiftx.md) |  |
| [`D3CurveETShiftY`](d3curveetshifty.md) |  |
| [`D3CurveETSize`](d3curveetsize.md) |  |
| [`D3CurveETStrOut`](d3curveetstrout.md) |  |
| [`D3CurveETTxt`](d3curveettxt.md) |  |
| [`D3CurveETUndl`](d3curveetundl.md) |  |
| [`D3CurveExtIsoLineColor`](d3curveextisolinecolor.md) |  |
| [`D3CurveExtIsoLineColRGB`](d3curveextisolinecolrgb.md) |  |
| [`D3CurveExtIsoLineInterval`](d3curveextisolineinterval.md) |  |
| [`D3CurveExtIsoLineType`](d3curveextisolinetype.md) |  |
| [`D3CurveExtIsoLineWidth`](d3curveextisolinewidth.md) |  |
| [`D3CurveExtIsoValNo`](d3curveextisovalno.md) |  |
| [`D3CurveExtIsoValues`](d3curveextisovalues.md) |  |
| [`D3CurveFGColor`](d3curvefgcolor.md) |  |
| [`D3CurveFGColRGB`](d3curvefgcolrgb.md) |  |
| [`D3CurveFGrid`](d3curvefgrid.md) |  |
| [`D3CurveFilling`](d3curvefilling.md) |  |
| [`D3CurveFrameBackFMode`](d3curveframebackfmode.md) |  |
| [`D3CurveFrameBackFVariant`](d3curveframebackfvariant.md) |  |
| [`D3CurveFrameBkColor`](d3curveframebkcolor.md) |  |
| [`D3CurveFrameBkColRGB`](d3curveframebkcolrgb.md) |  |
| [`D3CurveFrameBkColRGB2`](d3curveframebkcolrgb2.md) |  |
| [`D3CurveFrameDeltaX`](d3curveframedeltax.md) |  |
| [`D3CurveFrameDeltaX`](d3curveframedeltax-2.md) |  |
| [`D3CurveFrameHeight`](d3curveframeheight.md) |  |
| [`D3CurveFrameLnColor`](d3curveframelncolor.md) |  |
| [`D3CurveFrameLnColRGB`](d3curveframelncolrgb.md) |  |
| [`D3CurveFrameLnType`](d3curveframelntype.md) |  |
| [`D3CurveFrameLnWidth`](d3curveframelnwidth.md) |  |
| [`D3CurveFrameWidth`](d3curveframewidth.md) |  |
| [`D3CurveGridBegin`](d3curvegridbegin.md) |  |
| [`D3CurveGridCalc`](d3curvegridcalc.md) |  |
| [`D3CurveGridEnd`](d3curvegridend.md) |  |
| [`D3CurveGridNo`](d3curvegridno.md) |  |
| [`D3CurveHidden`](d3curvehidden.md) |  |
| [`D3CurveInterp`](d3curveinterp.md) |  |
| [`D3CurveInterv`](d3curveinterv.md) |  |
| [`D3CurveIsoChn`](d3curveisochn.md) |  |
| [`D3CurveIsoColor`](d3curveisocolor.md) |  |
| [`D3CurveIsoColRGB`](d3curveisocolrgb.md) |  |
| [`D3CurveIsoInterv`](d3curveisointerv.md) |  |
| [`D3CurveIsolines`](d3curveisolines.md) |  |
| [`D3CurveIsoLType`](d3curveisoltype.md) |  |
| [`D3CurveIsoLWidth`](d3curveisolwidth.md) |  |
| [`D3CurveIsoType`](d3curveisotype.md) |  |
| [`D3CurveIsoVal`](d3curveisoval.md) |  |
| [`D3CurveIsoValNo`](d3curveisovalno.md) |  |
| [`D3CurveIsoValues`](d3curveisovalues.md) |  |
| [`D3CurveLegDrawT`](d3curvelegdrawt.md) | Valid names: D3CurveLegDrawT, D3CurveLegDraw |
| [`D3CurveLineType`](d3curvelinetype.md) |  |
| [`D3CurveMarkColor`](d3curvemarkcolor.md) |  |
| [`D3CurveMarkColorAuto`](d3curvemarkcolorauto.md) |  |
| [`D3CurveMarkColorRGB`](d3curvemarkcolorrgb.md) |  |
| [`D3CurveMarkFillColor`](d3curvemarkfillcolor.md) |  |
| [`D3CurveMarkFillColorAuto`](d3curvemarkfillcolorauto.md) |  |
| [`D3CurveMarkFillColorRGB`](d3curvemarkfillcolorrgb.md) |  |
| [`D3CurveMarkLineWidth`](d3curvemarklinewidth.md) |  |
| [`D3CurveMarkSize`](d3curvemarksize.md) |  |
| [`D3CurveMarkType`](d3curvemarktype.md) |  |
| [`D3CurveMassive`](d3curvemassive.md) |  |
| [`D3CurveNoMax`](d3curvenomax.md) |  |
| [`D3CurveObj`](d3curveobj.md) |  |
| [`D3CurvePalColor`](d3curvepalcolor.md) |  |
| [`D3CurvePalColRGB`](d3curvepalcolrgb.md) |  |
| [`D3CurvePalLine`](d3curvepalline.md) |  |
| [`D3CurvePalLType`](d3curvepalltype.md) |  |
| [`D3CurvePalNo`](d3curvepalno.md) |  |
| [`D3CurvePalWidth`](d3curvepalwidth.md) |  |
| [`D3CurveRedMode`](d3curveredmode.md) |  |
| [`D3CurveRedTol`](d3curveredtol.md) |  |
| [`D3CurveSpecColor`](d3curvespeccolor.md) |  |
| [`D3CurveSpecCRGB`](d3curvespeccrgb.md) |  |
| [`D3CurveSpecInter`](d3curvespecinter.md) |  |
| [`D3CurveSpecLType`](d3curvespecltype.md) |  |
| [`D3CurveSpecLWid`](d3curvespeclwid.md) |  |
| [`D3CurveSpecOffs`](d3curvespecoffs.md) |  |
| [`D3CurveSpecWidth`](d3curvespecwidth.md) |  |
| [`D3CurveStruc`](d3curvestruc.md) |  |
| [`D3CurveStruc1`](d3curvestruc1.md) |  |
| [`D3CurveSurfType`](d3curvesurftype.md) |  |
| [`D3CurveSymAng`](d3curvesymang.md) |  |
| [`D3CurveSymBackColor`](d3curvesymbackcolor.md) |  |
| [`D3CurveSymBackColorRGB`](d3curvesymbackcolorrgb.md) |  |
| [`D3CurveSymBold`](d3curvesymbold.md) |  |
| [`D3CurveSymBType`](d3curvesymbtype.md) |  |
| [`D3CurveSymCFormat`](d3curvesymcformat.md) |  |
| [`D3CurveSymChn`](d3curvesymchn.md) |  |
| [`D3CurveSymChnName`](d3curvesymchnname.md) |  |
| [`D3CurveSymColor`](d3curvesymcolor.md) | Valid names: D3CurveSymColor, D3CSCo |
| [`D3CurveSymColRGB`](d3curvesymcolrgb.md) |  |
| [`D3CurveSymCType`](d3curvesymctype.md) |  |
| [`D3CurveSymEType`](d3curvesymetype.md) |  |
| [`D3CurveSymFont`](d3curvesymfont.md) | Valid names: D3CurveSymFont, D3CSFnt |
| [`D3CurveSymFrame`](d3curvesymframe.md) |  |
| [`D3CurveSymFType`](d3curvesymftype.md) |  |
| [`D3CurveSymHdNo`](d3curvesymhdno.md) |  |
| [`D3CurveSymHdType`](d3curvesymhdtype.md) |  |
| [`D3CurveSymIdxChn`](d3curvesymidxchn.md) |  |
| [`D3CurveSymIdxChnName`](d3curvesymidxchnname.md) |  |
| [`D3CurveSymIFormat`](d3curvesymiformat.md) |  |
| [`D3CurveSymItal`](d3curvesymital.md) |  |
| [`D3CurveSymNType`](d3curvesymntype.md) |  |
| [`D3CurveSymPFormat`](d3curvesympformat.md) |  |
| [`D3CurveSymPosTyp`](d3curvesympostyp.md) |  |
| [`D3CurveSymPtType`](d3curvesympttype.md) |  |
| [`D3CurveSymRelPos`](d3curvesymrelpos.md) |  |
| [`D3CurveSymRMode`](d3curvesymrmode.md) |  |
| [`D3CurveSymRType`](d3curvesymrtype.md) |  |
| [`D3CurveSymSepar`](d3curvesymsepar.md) |  |
| [`D3CurveSymSize`](d3curvesymsize.md) | Valid names: D3CurveSymSize, D3CSSz |
| [`D3CurveSymStrOut`](d3curvesymstrout.md) | Valid names: D3CurveSymStrOut, D3CSSt |
| [`D3CurveSymType`](d3curvesymtype.md) |  |
| [`D3CurveSymUndl`](d3curvesymundl.md) |  |
| [`D3CurveSymXDelt`](d3curvesymxdelt.md) |  |
| [`D3CurveSymXFormat`](d3curvesymxformat.md) |  |
| [`D3CurveSymXType`](d3curvesymxtype.md) |  |
| [`D3CurveSymYDelt`](d3curvesymydelt.md) |  |
| [`D3CurveSymYFormat`](d3curvesymyformat.md) | Valid names: D3CurveSymYFormat, D3CurveSymFormat |
| [`D3CurveSymYType`](d3curvesymytype.md) |  |
| [`D3CurveSymZDelt`](d3curvesymzdelt.md) |  |
| [`D3CurveSymZFormat`](d3curvesymzformat.md) |  |
| [`D3CurveSymZType`](d3curvesymztype.md) |  |
| [`D3CurveTxt`](d3curvetxt.md) |  |
| [`D3CurveTxtAlignment`](d3curvetxtalignment.md) |  |
| [`D3CurveTxtBold`](d3curvetxtbold.md) |  |
| [`D3CurveTxtColor`](d3curvetxtcolor.md) |  |
| [`D3CurveTxtColorRGB`](d3curvetxtcolorrgb.md) |  |
| [`D3CurveTxtFont`](d3curvetxtfont.md) |  |
| [`D3CurveTxtItal`](d3curvetxtital.md) |  |
| [`D3CurveTxtSize`](d3curvetxtsize.md) |  |
| [`D3CurveTxtStrOut`](d3curvetxtstrout.md) |  |
| [`D3CurveTxtUndl`](d3curvetxtundl.md) |  |
| [`D3CurveType`](d3curvetype.md) |  |
| [`D3CurveVAng`](d3curvevang.md) |  |
| [`D3CurveVBegin`](d3curvevbegin.md) |  |
| [`D3CurveVColor`](d3curvevcolor.md) |  |
| [`D3CurveVColorRGB`](d3curvevcolorrgb.md) |  |
| [`D3CurveVComp`](d3curvevcomp.md) |  |
| [`D3CurveVConst`](d3curvevconst.md) |  |
| [`D3CurveVConstDef`](d3curvevconstdef.md) |  |
| [`D3CurveVDef`](d3curvevdef.md) |  |
| [`D3CurveVEnd`](d3curvevend.md) |  |
| [`D3CurveVFactor`](d3curvevfactor.md) |  |
| [`D3CurveVHead`](d3curvevhead.md) |  |
| [`D3CurveVHeadSize`](d3curvevheadsize.md) |  |
| [`D3CurveVHeadVar`](d3curvevheadvar.md) |  |
| [`D3CurveVInterv`](d3curvevinterv.md) |  |
| [`D3CurveVLineType`](d3curvevlinetype.md) |  |
| [`D3CurveVMark`](d3curvevmark.md) |  |
| [`D3CurveVPlane`](d3curvevplane.md) |  |
| [`D3CurveVPlaneTyp`](d3curvevplanetyp.md) |  |
| [`D3CurveVScal`](d3curvevscal.md) |  |
| [`D3CurveVType`](d3curvevtype.md) |  |
| [`D3CurveVTypeInt`](d3curvevtypeint.md) |  |
| [`D3CurveVWidth`](d3curvevwidth.md) |  |
| [`D3CurveWaterType`](d3curvewatertype.md) |  |
| [`D3CurveWidth`](d3curvewidth.md) |  |
| [`D3DataType`](d3datatype.md) | Specifies whether the data is available in triplet or matrix form. |
| [`D3DigitDist`](d3digitdist.md) |  |
| [`D3Direc`](d3direc.md) |  |
| [`D3GridBegin`](d3gridbegin.md) | Specifies the minimum grid point. |
| [`D3GridCalc`](d3gridcalc.md) | Specifies how DIAdem determines the start value and the end value of a grid. |
| [`D3GridCalcAll`](d3gridcalcall.md) | Specifies whether DIAdem uses all points of a grid. |
| [`D3GridChn`](d3gridchn.md) | Specifies a data channel that contains the grid points. |
| [`D3GridEnd`](d3gridend.md) | Specifies the maximum grid point. |
| [`D3GridGen`](d3gridgen.md) | Specifies the origin of the points for generating the grid. |
| [`D3GridNo`](d3gridno.md) | Specifies the number of grid points. |
| [`D3GridPolyg`](d3gridpolyg.md) | Specifies how DIAdem calculates the polygon that limits the section to be evaluated. |
| [`D3GridPolygChn`](d3gridpolygchn.md) | Specifies the data channels that contain the x-values and y-values of the polygon. |
| [`D3GridPolygConv`](d3gridpolygconv.md) | Specifies whether DIAdem checks the polygon for convexity. |
| [`D3InterpMethChn`](d3interpmethchn.md) | Specifies the 3D interpolation method for input data in a triplet structure. |
| [`D3InterpMethMat`](d3interpmethmat.md) | Specifies the 3D interpolation method for input data that have a matrix structure. |
| [`D3InterpPara`](d3interppara.md) | Specifies the exponent p for the 3D interpolation procedure Inverse Distance . |
| [`D3IsolineBdry`](d3isolinebdry.md) | Specifies whether DIAdem uses a boundary curve to calculate the contour. |
| [`D3IsolineBdryCNo`](d3isolinebdrycno.md) | Specifies the data channels that contain the x and y-values of the boundary curve. |
| [`D3IsolineBdryIP`](d3isolinebdryip.md) | Specifies whether DIAdem interpolates the boundary curve in a contour line calculation. |
| [`D3IsolineBdryPol`](d3isolinebdrypol.md) | Specifies whether DIAdem calculates the boundary curve from value pairs or from the convex or non-convex hull. |
| [`D3IsolineBegin`](d3isolinebegin.md) | Specifies the minimum contour value. |
| [`D3IsolineCalc`](d3isolinecalc.md) | Specifies whether DIAdem calculates the start and end contour values. |
| [`D3IsolineChn`](d3isolinechn.md) | Specifies the data channel that contains the contour values. |
| [`D3IsolineCompare`](d3isolinecompare.md) | Receives a constant component of the contour line calculation. |
| [`D3IsolineEnd`](d3isolineend.md) | Specifies the maximum contour value. |
| [`D3IsolineNo`](d3isolineno.md) | Specifies the number of contour values. |
| [`D3IsolineSource`](d3isolinesource.md) | Specifies whether DIAdem calculates the contour values or whether DIAdem takes the contour values from a data channel. |
| [`D3LegAngle`](d3legangle.md) |  |
| [`D3LegBackColor`](d3legbackcolor.md) |  |
| [`D3LegBackFMode`](d3legbackfmode.md) |  |
| [`D3LegBackFVariant`](d3legbackfvariant.md) |  |
| [`D3LegBackRGB`](d3legbackrgb.md) |  |
| [`D3LegBackRGB2`](d3legbackrgb2.md) |  |
| [`D3LegClip`](d3legclip.md) |  |
| [`D3LegDraw`](d3legdraw.md) |  |
| [`D3LegFirstOnly`](d3legfirstonly.md) |  |
| [`D3LegFrame`](d3legframe.md) |  |
| [`D3LegFrameCol`](d3legframecol.md) |  |
| [`D3LegFrameColRGB`](d3legframecolrgb.md) |  |
| [`D3LegFrameWidth`](d3legframewidth.md) |  |
| [`D3LegGridLines`](d3leggridlines.md) |  |
| [`D3LegMove`](d3legmove.md) |  |
| [`D3LegNo`](d3legno.md) |  |
| [`D3LegOrient`](d3legorient.md) |  |
| [`D3LegPAll`](d3legpall.md) |  |
| [`D3LegPAngle`](d3legpangle.md) |  |
| [`D3LegPBackColor`](d3legpbackcolor.md) |  |
| [`D3LegPBackFMode`](d3legpbackfmode.md) |  |
| [`D3LegPBackFVariant`](d3legpbackfvariant.md) |  |
| [`D3LegPBackRGB`](d3legpbackrgb.md) |  |
| [`D3LegPBackRGB2`](d3legpbackrgb2.md) |  |
| [`D3LegPClip`](d3legpclip.md) |  |
| [`D3LegPDraw`](d3legpdraw.md) |  |
| [`D3LegPFrame`](d3legpframe.md) |  |
| [`D3LegPFrameCol`](d3legpframecol.md) |  |
| [`D3LegPFrameCRGB`](d3legpframecrgb.md) |  |
| [`D3LegPFrameWidth`](d3legpframewidth.md) |  |
| [`D3LegPMove`](d3legpmove.md) |  |
| [`D3LegPOrient`](d3legporient.md) |  |
| [`D3LegPositionType`](d3legpositiontype.md) |  |
| [`D3LegPosSysRelatedX`](d3legpossysrelatedx.md) |  |
| [`D3LegPosSysRelatedY`](d3legpossysrelatedy.md) |  |
| [`D3LegPosX`](d3legposx.md) |  |
| [`D3LegPosY`](d3legposy.md) |  |
| [`D3LegPPositionType`](d3legppositiontype.md) |  |
| [`D3LegPPosSysRelatedX`](d3legppossysrelatedx.md) |  |
| [`D3LegPPosSysRelatedY`](d3legppossysrelatedy.md) |  |
| [`D3LegPPosX`](d3legpposx.md) |  |
| [`D3LegPPosY`](d3legpposy.md) |  |
| [`D3LegPRelPos`](d3legprelpos.md) |  |
| [`D3LegPSclDomain`](d3legpscldomain.md) |  |
| [`D3LegPSclFirstLastOnly`](d3legpsclfirstlastonly.md) |  |
| [`D3LegPSclFormat`](d3legpsclformat.md) |  |
| [`D3LegPSclRed`](d3legpsclred.md) |  |
| [`D3LegPSclType`](d3legpscltype.md) |  |
| [`D3LegPSclValType`](d3legpsclvaltype.md) |  |
| [`D3LegPSizeGlX`](d3legpsizeglx.md) |  |
| [`D3LegPSizeGlY`](d3legpsizegly.md) |  |
| [`D3LegPSizeLoX`](d3legpsizelox.md) |  |
| [`D3LegPSizeLoY`](d3legpsizeloy.md) |  |
| [`D3LegPSizeType`](d3legpsizetype.md) |  |
| [`D3LegPSymDist`](d3legpsymdist.md) |  |
| [`D3LegPSymFrame`](d3legpsymframe.md) |  |
| [`D3LegPSymSize`](d3legpsymsize.md) |  |
| [`D3LegPSymType`](d3legpsymtype.md) |  |
| [`D3LegPTAngle`](d3legptangle.md) |  |
| [`D3LegPTFrame`](d3legptframe.md) |  |
| [`D3LegPTitle`](d3legptitle.md) |  |
| [`D3LegPTRelPos`](d3legptrelpos.md) |  |
| [`D3LegPTSize`](d3legptsize.md) |  |
| [`D3LegPTTxtBold`](d3legpttxtbold.md) | Valid names: D3LegPTTxtBold, D3LPTTB |
| [`D3LegPTTxtCol`](d3legpttxtcol.md) | Valid names: D3LegPTTxtCol, D3LPTTC |
| [`D3LegPTTxtColRGB`](d3legpttxtcolrgb.md) |  |
| [`D3LegPTTxtFont`](d3legpttxtfont.md) | Valid names: D3LegPTTxtFont, D3LPTTF |
| [`D3LegPTTxtFrame`](d3legpttxtframe.md) |  |
| [`D3LegPTTxtItal`](d3legpttxtital.md) | Valid names: D3LegPTTxtItal, D3LPTTI |
| [`D3LegPTTxtSize`](d3legpttxtsize.md) | Valid names: D3LegPTTxtSize, D3LPTTSz |
| [`D3LegPTTxtStrOut`](d3legpttxtstrout.md) | Valid names: D3LegPTTxtStrOut, D3LPTTSO |
| [`D3LegPTTxtSzAut`](d3legpttxtszaut.md) |  |
| [`D3LegPTTxtUndl`](d3legpttxtundl.md) | Valid names: D3LegPTTxtUndl, D3LPTTU |
| [`D3LegPTxtBold`](d3legptxtbold.md) | Valid names: D3LegPTxtBold, D3LPTB |
| [`D3LegPTxtCol`](d3legptxtcol.md) | Valid names: D3LegPTxtCol, D3LPTC |
| [`D3LegPTxtColAut`](d3legptxtcolaut.md) |  |
| [`D3LegPTxtColRGB`](d3legptxtcolrgb.md) |  |
| [`D3LegPTxtFont`](d3legptxtfont.md) | Valid names: D3LegPTxtFont, D3LPTF |
| [`D3LegPTxtItal`](d3legptxtital.md) | Valid names: D3LegPTxtItal, D3LPTI |
| [`D3LegPTxtPos`](d3legptxtpos.md) |  |
| [`D3LegPTxtSize`](d3legptxtsize.md) | Valid names: D3LegPTxtSize, D3LPTSz |
| [`D3LegPTxtSizeAut`](d3legptxtsizeaut.md) |  |
| [`D3LegPTxtStrOut`](d3legptxtstrout.md) | Valid names: D3LegPTxtStrOut, D3LPTSO |
| [`D3LegPTxtUndl`](d3legptxtundl.md) | Valid names: D3LegPTxtUndl, D3LPTU |
| [`D3LegRelPos`](d3legrelpos.md) |  |
| [`D3LegSizeGlX`](d3legsizeglx.md) |  |
| [`D3LegSizeGlY`](d3legsizegly.md) |  |
| [`D3LegSizeLoX`](d3legsizelox.md) |  |
| [`D3LegSizeLoY`](d3legsizeloy.md) |  |
| [`D3LegSizeType`](d3legsizetype.md) |  |
| [`D3LegSymDist`](d3legsymdist.md) |  |
| [`D3LegSymFrame`](d3legsymframe.md) |  |
| [`D3LegSymSize`](d3legsymsize.md) |  |
| [`D3LegTAngle`](d3legtangle.md) |  |
| [`D3LegTFrame`](d3legtframe.md) |  |
| [`D3LegTitle`](d3legtitle.md) |  |
| [`D3LegTitleA`](d3legtitlea.md) |  |
| [`D3LegTRelPos`](d3legtrelpos.md) |  |
| [`D3LegTSize`](d3legtsize.md) |  |
| [`D3LegTTxtBold`](d3legttxtbold.md) | Valid names: D3LegTTxtBold, D3LTTB |
| [`D3LegTTxtCol`](d3legttxtcol.md) | Valid names: D3LegTTxtCol, D3LTTC |
| [`D3LegTTxtColRGB`](d3legttxtcolrgb.md) |  |
| [`D3LegTTxtFont`](d3legttxtfont.md) | Valid names: D3LegTTxtFont, D3LTTF |
| [`D3LegTTxtFrame`](d3legttxtframe.md) |  |
| [`D3LegTTxtItal`](d3legttxtital.md) | Valid names: D3LegTTxtItal, D3LTTI |
| [`D3LegTTxtSize`](d3legttxtsize.md) | Valid names: D3LegTTxtSize, D3LTTSz |
| [`D3LegTTxtStrOut`](d3legttxtstrout.md) | Valid names: D3LegTTxtStrOut, D3LTTSO |
| [`D3LegTTxtSzAut`](d3legttxtszaut.md) |  |
| [`D3LegTTxtUndl`](d3legttxtundl.md) | Valid names: D3LegTTxtUndl, D3LTTU |
| [`D3LegTxtBold`](d3legtxtbold.md) | Valid names: D3LegTxtBold, D3LTB |
| [`D3LegTxtClip`](d3legtxtclip.md) |  |
| [`D3LegTxtCol`](d3legtxtcol.md) | Valid names: D3LegTxtCol, D3LTC |
| [`D3LegTxtColAut`](d3legtxtcolaut.md) |  |
| [`D3LegTxtColRGB`](d3legtxtcolrgb.md) |  |
| [`D3LegTxtFont`](d3legtxtfont.md) | Valid names: D3LegTxtFont, D3LTF |
| [`D3LegTxtFrame`](d3legtxtframe.md) |  |
| [`D3LegTxtFree`](d3legtxtfree.md) |  |
| [`D3LegTxtFreeA`](d3legtxtfreea.md) |  |
| [`D3LegTxtItal`](d3legtxtital.md) | Valid names: D3LegTxtItal, D3LTI |
| [`D3LegTxtPos`](d3legtxtpos.md) |  |
| [`D3LegTxtRelWidth`](d3legtxtrelwidth.md) |  |
| [`D3LegTxtSize`](d3legtxtsize.md) | Valid names: D3LegTxtSize, D3LTSz |
| [`D3LegTxtSizeAut`](d3legtxtsizeaut.md) |  |
| [`D3LegTxtStrOut`](d3legtxtstrout.md) | Valid names: D3LegTxtStrOut, D3LTSO |
| [`D3LegTxtType`](d3legtxttype.md) |  |
| [`D3LegTxtTypeA`](d3legtxttypea.md) |  |
| [`D3LegTxtUndl`](d3legtxtundl.md) | Valid names: D3LegTxtUndl, D3LTU |
| [`D3LegTxtWordWrap`](d3legtxtwordwrap.md) |  |
| [`D3LineColor`](d3linecolor.md) |  |
| [`D3LineColorRGB`](d3linecolorrgb.md) |  |
| [`D3MaximumZValue`](d3maximumzvalue.md) | Specifies the top limit of the z-value to check. |
| [`D3MinimumZValue`](d3minimumzvalue.md) | Specifies the bottom limit of the z-value to check. |
| [`D3NodeDist`](d3nodedist.md) | Specifies the size of the frame as a percentage of the x and y-expansion of the input data where DIAdem searches for nodes. |
| [`D3NodeMeth`](d3nodemeth.md) | Specifies which points DIAdem uses for the interpolation of an evaluation point. |
| [`D3NodeNo`](d3nodeno.md) | Specifies the number of neighboring points to be used. |
| [`D3NodeSel`](d3nodesel.md) | Specifies how DIAdem determines the interpolation points for the 3D interpolation. |
| [`D3PartialLoadMinNumberOfPoints`](d3partialloadminnumberofpoints.md) | Specifies the number of measurement points that must belong to a partial load so that this value is valid, in a characteristic diagram with partial load structure in DIAdem REPORT. |
| [`D3PartialLoadToleranceAbsolute`](d3partialloadtoleranceabsolute.md) | Specifies the maximum absolute deviation of the x-value within a partial load, in a characteristic diagram with partial load structure in DIAdem REPORT. |
| [`D3PartialLoadToleranceRelative`](d3partialloadtolerancerelative.md) | Valid names: D3PartialLoadToleranceRelative, D3PartialLoadTolerance |
| [`D3PartialLoadToleranceType`](d3partialloadtolerancetype.md) | Specifies whether you define the tolerance as a percentage of the entire x-area or as the absolute x-area, in a characteristic diagram with partial load structure in DIAdem REPORT. Points whose x-values lie outside the tolerance are invalid values of the partial load. |
| [`D3PlaneBackColor`](d3planebackcolor.md) |  |
| [`D3PlaneBackRGB`](d3planebackrgb.md) |  |
| [`D3PlaneColor`](d3planecolor.md) |  |
| [`D3PlaneColorRGB`](d3planecolorrgb.md) |  |
| [`D3PlaneInterv`](d3planeinterv.md) |  |
| [`D3PlaneLineType`](d3planelinetype.md) |  |
| [`D3PlaneOffs`](d3planeoffs.md) |  |
| [`D3PlaneTypeXY`](d3planetypexy.md) |  |
| [`D3PlaneTypeXZ`](d3planetypexz.md) |  |
| [`D3PlaneTypeYZ`](d3planetypeyz.md) |  |
| [`D3PlaneWidth`](d3planewidth.md) |  |
| [`D3SearchMode`](d3searchmode.md) | Specifies a condition. |
| [`D3StrucIn`](d3strucin.md) | Specifies whether the input data is in triplets or matrices. |
| [`D3StrucOut`](d3strucout.md) | Specifies whether DIAdem displays the result data in triplets or in matrices. |
| [`D3SubMatColumn`](d3submatcolumn.md) | Specifies which columns to copy from a submatrix. |
| [`D3SubMatRow`](d3submatrow.md) | Specifies which rows to copy from a submatrix. |
| [`D3SubMatTranspos`](d3submattranspos.md) | Specifies whether DIAdem transposes and saves rows and columns in a submatrix. |
| [`D3TabAng`](d3tabang.md) |  |
| [`D3TabAutoScal`](d3tabautoscal.md) |  |
| [`D3TabBackColor`](d3tabbackcolor.md) |  |
| [`D3TabBackFMode`](d3tabbackfmode.md) |  |
| [`D3TabBackFVariant`](d3tabbackfvariant.md) |  |
| [`D3TabBackRGB`](d3tabbackrgb.md) |  |
| [`D3TabBackRGB2`](d3tabbackrgb2.md) |  |
| [`D3TabBegin`](d3tabbegin.md) |  |
| [`D3TabBold`](d3tabbold.md) |  |
| [`D3TabBottom`](d3tabbottom.md) |  |
| [`D3TabChnX`](d3tabchnx.md) |  |
| [`D3TabChnXName`](d3tabchnxname.md) |  |
| [`D3TabChnY`](d3tabchny.md) |  |
| [`D3TabChnYName`](d3tabchnyname.md) |  |
| [`D3TabChnZ`](d3tabchnz.md) |  |
| [`D3TabChnZName`](d3tabchnzname.md) |  |
| [`D3TabColor`](d3tabcolor.md) | Valid names: D3TabColor, D3TCo |
| [`D3TabColorRGB`](d3tabcolorrgb.md) |  |
| [`D3TabEnd`](d3tabend.md) |  |
| [`D3TabFont`](d3tabfont.md) | Valid names: D3TabFont, D3TF |
| [`D3TabFormat`](d3tabformat.md) |  |
| [`D3TabGrid`](d3tabgrid.md) |  |
| [`D3TabHideZeroVal`](d3tabhidezeroval.md) |  |
| [`D3TabItal`](d3tabital.md) |  |
| [`D3TabLeft`](d3tableft.md) |  |
| [`D3TabLineWidth`](d3tablinewidth.md) |  |
| [`D3TabRelPos`](d3tabrelpos.md) |  |
| [`D3TabRight`](d3tabright.md) |  |
| [`D3TabSize`](d3tabsize.md) | Valid names: D3TabSize, D3TSz |
| [`D3TabStrOut`](d3tabstrout.md) | Valid names: D3TabStrOut, D3TSo |
| [`D3TabTop`](d3tabtop.md) |  |
| [`D3TabTxt`](d3tabtxt.md) |  |
| [`D3TabTxtArea`](d3tabtxtarea.md) |  |
| [`D3TabTxtAutoScal`](d3tabtxtautoscal.md) |  |
| [`D3TabTxtBold`](d3tabtxtbold.md) | Valid names: D3TabTxtBold, D3TTB |
| [`D3TabTxtColor`](d3tabtxtcolor.md) | Valid names: D3TabTxtColor, D3TTCo |
| [`D3TabTxtColorRGB`](d3tabtxtcolorrgb.md) |  |
| [`D3TabTxtField`](d3tabtxtfield.md) |  |
| [`D3TabTxtFont`](d3tabtxtfont.md) | Valid names: D3TabTxtFont, D3TTF |
| [`D3TabTxtItal`](d3tabtxtital.md) |  |
| [`D3TabTxtSize`](d3tabtxtsize.md) | Valid names: D3TabTxtSize, D3TTSz |
| [`D3TabTxtStrOut`](d3tabtxtstrout.md) | Valid names: D3TabTxtStrOut, D3TTSo |
| [`D3TabTxtUndl`](d3tabtxtundl.md) | Valid names: D3TabTxtUndl, D3TTU |
| [`D3TabUndl`](d3tabundl.md) |  |
| [`D3TripletDistribution`](d3tripletdistribution.md) | Specifies whether the triplet data is distributed free or in a partial load structure. This setting specifies the interpolation mode of the z-values. If you enable this setting, DIAdem lays y-z-splines with regular interpolation points in y-direction through the points of every partial load. Then DIAdem lays x-z-splines through the interpolation points in x-direction. A partial load is made up of points with x-values that lie in the specified tolerance range. |
| [`Data`](data.md) | Specifies the data object that provides access to the subobjects, methods, and properties for working with internal data. |
| [`DataArrayDrv`](dataarraydrv.md) | Specifies the path where DIAdem saves virtual data. |
| [`DataChanged`](datachanged.md) | Receives information about whether the internal data area contains modified data. Use the DataChangedClear command to mark the internal data area as unchanged. |
| [`DataDrvLibr`](datadrvlibr.md) |  |
| [`DataDrvUser`](datadrvuser.md) | Valid names: DataDrvUser, DataDrv |
| [`DataExtension`](dataextension.md) | Specifies the filename extension for data files. |
| [`DataFile`](datafile.md) | Valid names: DataFile, DatFile |
| [`DataFileCode`](datafilecode.md) | Specifies the coding procedure for DAT data files. By default DIAdem saves the data file in Unicode . |
| [`DataFileLst`](datafilelst.md) | Receives the list of files found. |
| [`DataFileLstLen`](datafilelstlen.md) | Receives the number of files found. |
| [`DataFileLstMode`](datafilelstmode.md) | Specifies whether you store the names of the selected files with absolute paths or without paths. |
| [`DataFileName`](datafilename.md) | Specifies the name of a data file with the filename extension and the path. |
| [`DataLibrPath`](datalibrpath.md) | Specifies the current path of the NAVIGATOR library folder for data. |
| [`DataReadPath`](datareadpath.md) | Specifies the current read path for data. |
| [`DataSaveKey`](datasavekey.md) | Specifies whether DIAdem saves the data in columns or rows. |
| [`DataSaveType`](datasavetype.md) | Specifies the data type in which DIAdem saves DAT data. |
| [`DataSetAddTxt1`](datasetaddtxt1.md) |  |
| [`DataSetAddTxt2`](datasetaddtxt2.md) |  |
| [`DataSetAddTxt3`](datasetaddtxt3.md) |  |
| [`DataSetAuthor`](datasetauthor.md) |  |
| [`DataSetByteOrder`](datasetbyteorder.md) | Specifies the order of the bytes in binary files. |
| [`DataSetComment`](datasetcomment.md) | Specifies the data set comment. |
| [`DataSetCommentN`](datasetcommentn.md) | Specifies the name of the data set comment. |
| [`DataSetDate`](datasetdate.md) |  |
| [`DataSetDescript`](datasetdescript.md) |  |
| [`DataSetDTFormat`](datasetdtformat.md) | Specifies the time format in ASCII files. |
| [`DataSetMaxComm`](datasetmaxcomm.md) | Specifies the maximum number of comments in a header of a data set. |
| [`DataSetName`](datasetname.md) |  |
| [`DataSetNov`](datasetnov.md) |  |
| [`DataSetTime`](datasettime.md) |  |
| [`DataSetTitle`](datasettitle.md) |  |
| [`DataType`](datatype.md) |  |
| [`DataWritePath`](datawritepath.md) | Specifies the current write path for data. |
| [`DDEBlockNo`](ddeblockno.md) |  |
| [`DDELastError`](ddelasterror.md) |  |
| [`DDEPokeStr`](ddepokestr.md) |  |
| [`DDEReqValue`](ddereqvalue.md) |  |
| [`DDESaveMode`](ddesavemode.md) |  |
| [`DDETimeout`](ddetimeout.md) |  |
| [`DDEUseBuf`](ddeusebuf.md) |  |
| [`DebuggerAvailabl`](debuggeravailabl.md) |  |
| [`DebuggerDLL`](debuggerdll.md) | Contains the name and path of the debugger DLL. |
| [`DebuggerVersion`](debuggerversion.md) | Contains the debugger-DLL version. |
| [`DefaultFileExportFilter`](defaultfileexportfilter.md) | Defines the default file type for saving data. You can use all file types for which DataPlugins for storing data are registered in DIAdem. |
| [`DefaultFileImportFilter`](defaultfileimportfilter.md) | Defines the default file type for loading data. You can use all file types for which DataPlugins for loading data are registered in DIAdem. |
| [`DefaultValue`](defaultvalue.md) | Specifies the text which DIAdem uses in assignment channels when no text is assigned to the value. |
| [`DefFileName`](deffilename.md) | Specifies the name of a user variable collection file or of a user variable definition file. |
| [`DeleteAssignments`](deleteassignments.md) | Specifies that DIAdem deletes the assignments for the AssignmentChnToNumericChn command and replaces the numeric channel with the assignment channel for the ChnToAssignmentChn command and also that DIAdem deletes the channel from where the assignment texts originate. The default value of the variable is FALSE . |
| [`DeleteAssignmentsIP`](deleteassignmentsip.md) | Specifies whether DIAdem replaces the assignment channel with the numeric channel. The default value of the variable is FALSE , so that DIAdem retains the assignment channel and creates an additional numeric channel. |
| [`DeleteDuplicatesInPlace`](deleteduplicatesinplace.md) | Specifies that DIAdem stores the results in the original channels. DIAdem creates new channels by default. |
| [`DeleteDuplicatesMode`](deleteduplicatesmode.md) | Specifies which value DIAdem accepts from the dependent channels. |
| [`DeleteDuplicateTextsCaseSensitive`](deleteduplicatetextscasesensitive.md) | Specifies whether text channels in DIAdem are case sensitive. |
| [`DeleteDuplicateValuesToleranceType`](deleteduplicatevaluestolerancetype.md) | Specifies whether to define tolerance as a percentage or absolute or whether no tolerance is defined. The percentage value refers to the current channel value of the channel to be reduced. By default, DIAdem does not define a tolerance. |
| [`DeleteDuplicateValuesToleranceValue`](deleteduplicatevaluestolerancevalue.md) | Specifies the tolerance value as an absolute value or as a percentage. The percentage value refers to the current channel value of the channel to be reduced. By default, DIAdem does not define a tolerance. |
| [`DeleteTextChannel`](deletetextchannel.md) | Specifies that DIAdem deletes the text channel which contains the texts for the assignments. The default value of the variable is FALSE , so that DIAdem does not delete the channel. |
| [`DeskCalculationSet`](deskcalculationset.md) | Specifies the default file for the formula templates. |
| [`DeskData`](deskdata.md) | Specifies the name of the data file that DIAdem loads into the Data Portal when the program starts. |
| [`DeskDrv`](deskdrv.md) | Specifies the path with the folder from which DIAdem loads the desktop file. |
| [`DeskFile`](deskfile.md) | Specifies the name of the desktop file . |
| [`DeskPic`](deskpic.md) | Specifies the name of the REPORT layout that DIAdem loads when the program starts. |
| [`DesktopChanged`](desktopchanged.md) | Indicates whether you have changed the DIAdem desktop file. |
| [`DeskVIEW`](deskview.md) | Specifies the name of the VIEW layout that DIAdem loads when the program starts. |
| [`DlgState`](dlgstate.md) | Receives the status of a dialog box after you exit the dialog box. |
| [`DLLDevLstLength`](dlldevlstlength.md) | Specifies the number of registered GPI drivers. |
| [`DRIDampingCoefficient`](dridampingcoefficient.md) | Specifies the damping coefficient if the DRI calculation is free. |
| [`DRIDirection`](dridirection.md) | Specifies the direction of the DRI calculation. If you do not set this parameter, DIAdem calculates the z-axis. |
| [`DRINaturalFrequency`](drinaturalfrequency.md) | Specifies the natural frequency of the dynamic system in rad/s if the DRI calculation is free. |
| [`DRIRes`](drires.md) | Receives the result of the DRI calculation. |
| [`DurationType`](durationtype.md) | Specifies whether DIAdem calculates the time-at-level from one section or several sections. |
| [`DXPeak`](dxpeak.md) | Specifies the interval width as a percentage of the x-range in which DIAdem determines the extreme values. |
| [`EditNoMax`](editnomax.md) | Specifies the maximum number of channels that DIAdem can read from a DAT file and can edit. |
| [`eInterFirstValue`](einterfirstvalue.md) | Specifies the first value as the data reduction. |
| [`eInterMaximum`](eintermaximum.md) | Specifies the maximum value of the specified interval for the data reduction. |
| [`eInterMeanValue`](eintermeanvalue.md) | Specifies the mean value of the specified interval for the data reduction. |
| [`eInterMinimum`](einterminimum.md) | Specifies the minimum of the specified interval for the data reduction. |
| [`EllipsoidGeometryType`](ellipsoidgeometrytype.md) | Specifies whether DIAdem assumes that the Earth is a sphere or ellipsoid according to the 1984 World Geodetic System (WGS 84). |
| [`EngineAvailable`](engineavailable.md) |  |
| [`EngineDLL`](enginedll.md) | Displays the name and path of the script engine DLL. |
| [`EngineVersion`](engineversion.md) | Displays the script engine DLL version. |
| [`EquidistantCheckMode`](equidistantcheckmode.md) | Specifies whether DIAdem checks all channels or only strictly monotonic channels. |
| [`ErrNo`](errno.md) |  |
| [`ErrorTxt`](errortxt.md) |  |
| [`ExBitsPerPixel`](exbitsperpixel.md) | Specifies the color depth in bits per pixel for a graphic that is to be exported. |
| [`ExBitsPerPixelA`](exbitsperpixela.md) | Specifies the color depth in bits per pixel for a graphic that is to be exported. |
| [`ExcelFileName`](excelfilename.md) | Specifies the Excel file that DIAdem opens. If you do not specify an Excel file, the command creates an Excel workbook with an empty worksheet named Sheet1 . |
| [`ExCompressType`](excompresstype.md) | Specifies the compression type of a graphic to be exported. |
| [`ExCompressTypeA`](excompresstypea.md) | Specifies the compression type of a graphic to be exported. |
| [`ExecOption`](execoption.md) | Specifies whether a script can execute functions of a DIAdem option. |
| [`ExFilename`](exfilename.md) | Specifies the name of a graphics file to be exported, with the filename extension and path. |
| [`ExHeight`](exheight.md) | Valid names: ExHeight, ExHeigth |
| [`ExProgressive`](exprogressive.md) | Specifies the number of display layers for a JPEG graphic. |
| [`ExQuality`](exquality.md) | Specifies the picture quality for a JPEG graphic. |
| [`ExShowImage`](exshowimage.md) | Specifies whether DIAdem opens the graphics file in an external graphics program after exporting it. |
| [`ExtEditorName`](exteditorname.md) | Specifies the name of an external text editor. |
| [`ExtendChnName`](extendchnname.md) | Specifies how DIAdem records channel references in dialog boxes and scripts. |
| [`ExtProgramArg`](extprogramarg.md) | Specifies the parameters that DIAdem uses to start an external program. |
| [`ExtProgramName`](extprogramname.md) | Specifies the name of an external program including the path. |
| [`ExType`](extype.md) | Specifies the format of a graphic to be exported, in DIAdem REPORT. |
| [`ExUseRatio`](exuseratio.md) | Specifies whether DIAdem maintains the height-width ratio in a graphic. |
| [`ExWidth`](exwidth.md) | Specifies the width in pixels of a graphic to be exported. |
| [`FFCVersion`](ffcversion.md) | Receives the version number of the FFC calculation routine. |
| [`FFTAmpl`](fftampl.md) | Specifies whether DIAdem calculates the amplitudes. |
| [`FFTAmplExt`](fftamplext.md) | Specifies whether DIAdem calculates third or octave analyses for the amplitudes. |
| [`FFTAmplFirst`](fftamplfirst.md) | Specifies whether DIAdem calculates the amplitude average or the autospectrum average. |
| [`FFTAmplType`](fftampltype.md) | Specifies the type of amplitude. |
| [`FFTAverageType`](fftaveragetype.md) | Specifies how DIAdem averages the amplitudes. |
| [`FFTCalc`](fftcalc.md) | Specifies whether DIAdem calculates the real and imaginary parts. |
| [`FFTCepstrum`](fftcepstrum.md) | Specifies whether DIAdem calculates the cepstrum. |
| [`FFTCoherence`](fftcoherence.md) | Specifies whether DIAdem calculates the coherence. |
| [`FFTCrossPhase`](fftcrossphase.md) | Specifies whether DIAdem calculates the phase spectrum of the cross spectra. |
| [`FFTCrossSpectr`](fftcrossspectr.md) | Specifies whether DIAdem calculates the cross spectrum. |
| [`FFTIndexChn`](fftindexchn.md) | In a multiple FFT this variable specifies whether DIAdem counts the calculated FFTs in a new index channel. |
| [`FFTIntervOverl`](fftintervoverl.md) | Specifies the overlapping of the time domains as a percentage of the interval length. |
| [`FFTIntervPara`](fftintervpara.md) | Specifies the settings for the time interval that you divide the data channel you want to analyze into. |
| [`FFTIntervUser`](fftintervuser.md) | Specifies the settings for the time intervals. |
| [`FFTNoV`](fftnov.md) | Specifies whether DIAdem uses NoValues for a data channel. |
| [`FFTPhase`](fftphase.md) | Specifies whether DIAdem calculates the phase spectrum. |
| [`FFTTransfctType`](ffttransfcttype.md) | Specifies whether DIAdem calculates the transfer function of the input signal and the output signal. |
| [`FFTTransPhase`](ffttransphase.md) | Specifies whether DIAdem calculates the phase spectrum of the transfer function. |
| [`FFTWndChn`](fftwndchn.md) | Specifies the data channel that contains the values of a user-defined window function. |
| [`FFTWndCorrectTyp`](fftwndcorrecttyp.md) | Specifies whether and how DIAdem corrects the damping effect of the window function on the amplitude. |
| [`FFTWndFct`](fftwndfct.md) | Specifies the window function of an FFT |
| [`FFTWndPara`](fftwndpara.md) | Specifies the parameters for parameter-related window functions. |
| [`FileChnBeginIdx`](filechnbeginidx.md) | Specifies the first value to be read in when DAT files are imported via header. |
| [`FileChnBeginVal`](filechnbeginval.md) | Specifies the start value or the offset of a data channel in an import of DAT files via header. |
| [`FileChnColWidthE`](filechncolwidthe.md) |  |
| [`FileChnColWidthP`](filechncolwidthp.md) |  |
| [`FileChnComment`](filechncomment.md) | Specifies the comment on the data channel when DAT files are imported via header. |
| [`FileChnDataFile`](filechndatafile.md) | Specifies the name and the extension of the data file that contains the bulk data from the import of DAT files via header. |
| [`FileChnDataStyle`](filechndatastyle.md) | Specifies the data type of the channel data when DAT files are imported via header. |
| [`FileChnDataType`](filechndatatype.md) | Specifies whether a data channel is implicit or explicit when you import DAT files via header. |
| [`FileChnDim`](filechndim.md) | Specifies the unit of a channel in the external header area when DAT files are imported via header. |
| [`FileChnFormat`](filechnformat.md) | Specifies the display format of the channel when DAT files are imported via header. |
| [`FileChnLength`](filechnlength.md) | Specifies the length of a data channel when DAT files are imported via header. |
| [`FileChnMonoKey`](filechnmonokey.md) | Specifies the monotony behavior of a data channel when DAT files are imported via header. |
| [`FileChnName`](filechnname.md) | Specifies the name of a data channel when DAT files are imported via header. |
| [`FileChnNo`](filechnno.md) | Specifies the number of channel headers when DAT files are imported via header. |
| [`FileChnNovInChn`](filechnnovinchn.md) | Specifies the NoValue value in a channel when DAT files are imported via header. |
| [`FileChnNovKey`](filechnnovkey.md) | Specifies whether a channel contains NoValues when DAT files are imported via header. |
| [`FileChnOffs`](filechnoffs.md) | Specifies the channel offset, that is the number of values between two channel values, when DAT files are imported via header. |
| [`FileChnOrder`](filechnorder.md) |  |
| [`FileChnSaveType`](filechnsavetype.md) | Specifies whether the data is ordered in channels or in blocks when you import DAT files via header. |
| [`FileChnStep`](filechnstep.md) | Specifies the value that DIAdem adds to the start value, or by which DIAdem multiplies the data when DAT files are imported via header. |
| [`FileChnValFormat`](filechnvalformat.md) |  |
| [`FileChnValMax`](filechnvalmax.md) | Valid names: FileChnValMax, FileChnMax |
| [`FileChnValMin`](filechnvalmin.md) | Valid names: FileChnValMin, FileChnMin |
| [`FileChnXMark`](filechnxmark.md) | Specifies the number of the x-channel if you load only specific values from a data channel when DAT files are imported via header. |
| [`FileCodingType`](filecodingtype.md) | Specifies with which code DIAdem generates or stores a file. |
| [`FileDataSaveSel`](filedatasavesel.md) | Specifies the name of the DAT file that you save selectively. |
| [`FileDlgASCIIName`](filedlgasciiname.md) | Specifies the ASCII file where you save the names of the files that you selected in the dialog box for opening and saving files. |
| [`FileDlgCaption`](filedlgcaption.md) | Specifies the dialog box caption. |
| [`FileDlgDir`](filedlgdir.md) | Receives the path of the file that you selected in the dialog box for loading and saving. |
| [`FileDlgExt`](filedlgext.md) | Receives the name extension of the file that you selected in the dialog box for loading and saving. |
| [`FileDlgExtension`](filedlgextension.md) | Specifies the filename extension. |
| [`FileDlgFile`](filedlgfile.md) | Specifies the name of the file that you selected in the dialog box for loading or saving. |
| [`FileDlgFileName`](filedlgfilename.md) | Receives a list of all the files, including the paths, that you select in the dialog box for loading or for saving. |
| [`FileDlgFilt`](filedlgfilt.md) | Specifies the file type. |
| [`FileDlgFilter`](filedlgfilter.md) | Specifies the file type when you load or save data. |
| [`FileDlgImpAction`](filedlgimpaction.md) | Receives the action you selected in the dialog box for loading. |
| [`FileDlgMultiSelect`](filedlgmultiselect.md) | Specifies whether one file or multiple files can be selected. The default value is FALSE and specifies that you can select only one file. |
| [`FileDlgName`](filedlgname.md) | Specifies a file. You can also specify the path and the filename extension. |
| [`FileDlgNameList`](filedlgnamelist.md) | Receives a field with all selected files including the path. |
| [`FileDlgPartial`](filedlgpartial.md) | Specifies whether to save only specified data or all data. |
| [`FileDlgPathKey`](filedlgpathkey.md) | Specifies whether DIAdem stores the names of the selected files with absolute paths or without paths in the ASCII file. The default value is FALSE which specifies that DIAdem does not save the absolute path as well. |
| [`FileDlgReduce`](filedlgreduce.md) | Receives information on whether you loaded the data reduced or complete. |
| [`FileExportFilter`](fileexportfilter.md) | Specifies the storage method you use to save data from the DIAdem Data Portal to a file. If you do not specify a storage method, DIAdem saves the data with the TDM DataPlugin. |
| [`FileFilter`](filefilter.md) | Specifies the name of the file filter. The name is the same name that DIAdem uses for loading and saving in the variables FileImportFilter and FileExportFilter . |
| [`FileFilterPreset`](filefilterpreset.md) | Specifies the name of the file filter that DIAdem used the last time it loaded data to the empty DIAdem Data Portal. If you load data with another file filter you do not modify the value of the variable. |
| [`FileHdAddTxt1`](filehdaddtxt1.md) | Specifies a variable that can be used for any additional information about the data set when DAT files are imported via header. |
| [`FileHdAddTxt2`](filehdaddtxt2.md) | Specifies a variable that can be used for any additional information about the data set when DAT files are imported via header. |
| [`FileHdAddTxt3`](filehdaddtxt3.md) | Specifies a variable that can be used for any additional information about the data set when DAT files are imported via header. |
| [`FileHdASCIIPtr`](filehdasciiptr.md) | Receives the information which value of an ASCII row DIAdem should import to a data channel when DAT files are imported via header. |
| [`FileHdASCIISep`](filehdasciisep.md) | Receives the character that separates the single values of ASCII block data when DAT files are imported via header. |
| [`FileHdAuthor`](filehdauthor.md) | Receives the author of the data set when DAT files are imported via header. |
| [`FileHdByteOrder`](filehdbyteorder.md) | Receives the byte order of binary dat when DAT files are imported via header. |
| [`FileHdComment`](filehdcomment.md) | Receives the comments of the data set when DAT files are imported via header. |
| [`FileHdCommentN`](filehdcommentn.md) | Receives the descriptive comments on the data set when DAT files are imported via header. |
| [`FileHdDate`](filehddate.md) | Receives the date of the last storage of the data set when DAT files are imported via header. |
| [`FileHdDecChar`](filehddecchar.md) | Receives the decimal symbol used in ASCII files when DAT files are imported via header. |
| [`FileHdDTFormat`](filehddtformat.md) | Receives the time format used in ASCII files when DAT files are imported via header. |
| [`FileHdExpChar`](filehdexpchar.md) | Receives the exponential character used in ASCII files when DAT files are imported via header. |
| [`FileHdNov`](filehdnov.md) | Receives the NoValue value of the data set when DAT files are imported via header. |
| [`FileHdTime`](filehdtime.md) | Receives the time of the last storage of the data set when DAT files are imported via header. |
| [`FileHdTitle`](filehdtitle.md) | Receives the name of the data set when DAT files are imported via header. |
| [`FileHdType`](filehdtype.md) | Receives the type of the data set when DAT files are imported via header. |
| [`FileImportFilter`](fileimportfilter.md) | Specifies the DataPlugin which DIAdem uses for loading a data file into the Data Portal. |
| [`FileLine`](fileline.md) | Valid names: FileLine, WriteLine |
| [`FileLineNo`](filelineno.md) | Valid names: FileLineNo, ReadNo |
| [`FileLstFilter`](filelstfilter.md) | Specifies the information that DIAdem saves. The default value of the FileLstFilter variable is onlyFilenames . |
| [`FileLstMode`](filelstmode.md) | Specifies whether DIAdem overwrites the contents of the ASCII file or whether DIAdem appends new rows to the ASCII file. |
| [`FileLstName`](filelstname.md) | Specifies the path and the name of the ASCII file that DIAdem writes the filenames into. |
| [`FileMode`](filemode.md) | Valid names: FileMode, OpenMode |
| [`FileModification`](filemodification.md) | Specifies whether DIAdem prompts you to save modified files or settings when you close a panel or exit DIAdem. |
| [`FileName`](filename.md) | Valid names: FileName, ReadWriteFile, OpenName |
| [`FileOperation`](fileoperation.md) | Specifies whether you load a file or save a file. |
| [`FileSaveCompressedTDMHeader`](filesavecompressedtdmheader.md) | Specifies whether DIAdem compresses the meta data without any losses. |
| [`FileSaveDataType`](filesavedatatype.md) | Specifies how DIAdem determines the data format for TDM data. |
| [`FileTargetDevice`](filetargetdevice.md) | Specifies the DIAdem panel for which you load or save a file. |
| [`FiltBothWays`](filtbothways.md) |  |
| [`FiltCorrection`](filtcorrection.md) | Specifies whether DIAdem corrects the offset for lowpass filters when it runs digital filtering on a time signal with recursive IIR filters. |
| [`FiltDegree`](filtdegree.md) | Specifies the filter degree for digital filtering with IIR filters. |
| [`FiltLimit`](filtlimit.md) | Specifies the 3 dB limit frequency of an IIR filter for highpass and lowpass. For allpass of an FIR filter, it specifies the frequency where the phase angle rotation reaches half the phase angle rotation of the overall system. |
| [`FiltLowLimit`](filtlowlimit.md) | Specifies the lower 3 dB-limit frequency for bandpass or bandstop. |
| [`FiltSamples`](filtsamples.md) | Specifies the number of values in the input signal that DIAdem calculates in the linear filter structure. |
| [`FiltStruc`](filtstruc.md) | Specifies the filter method. |
| [`FiltStyle`](filtstyle.md) | Specifies the filter type when an IIR filter method is used. |
| [`FiltType`](filttype.md) | Specifies the filter type. |
| [`FiltUppLimit`](filtupplimit.md) | Specifies the upper 3 dB-limit frequency for bandpass or bandstop. |
| [`FiltWave`](filtwave.md) | Specifies the ripple in the pass range for Chebyshev filtering. |
| [`FiltWndFct`](filtwndfct.md) | Specifies the window functions when DIAdem uses non-recursive FIR filters. |
| [`FiltZeroPhase`](filtzerophase.md) | Specifies whether DIAdem eliminates phase shifting in the filtered signal when IIR filters are used. |
| [`Fir100RemoveBias`](fir100removebias.md) | Specifies whether DIAdem eliminates the bias in FIR100 filtering. The default value is FALSE , which specifies that DIAdem does not remove the bias. |
| [`FIR100SampleType`](fir100sampletype.md) | Valid names: FIR100SampleType, FIR100OverSample |
| [`FloorIsNovalue`](floorisnovalue.md) | Specifies whether DIAdem replaces the value that corresponds to the SplitValue variable with NoValue or with the value of the SplitValue variable, in the result channels. |
| [`FmlArrowEndPtX`](fmlarrowendptx.md) |  |
| [`FmlArrowEndPtY`](fmlarrowendpty.md) |  |
| [`FmlArrowLnColor`](fmlarrowlncolor.md) |  |
| [`FmlArrowLnColRGB`](fmlarrowlncolrgb.md) |  |
| [`FmlArrowLnType`](fmlarrowlntype.md) |  |
| [`FmlArrowLnWidth`](fmlarrowlnwidth.md) |  |
| [`FmlArrowPTPos`](fmlarrowptpos.md) |  |
| [`FmlArrowStartPtX`](fmlarrowstartptx.md) |  |
| [`FmlArrowStartPtY`](fmlarrowstartpty.md) |  |
| [`FmlArrowSymbBeg`](fmlarrowsymbbeg.md) |  |
| [`FmlArrowSymbEnd`](fmlarrowsymbend.md) |  |
| [`FmlFrameBackFMode`](fmlframebackfmode.md) |  |
| [`FmlFrameBackFVariant`](fmlframebackfvariant.md) |  |
| [`FmlFrameBkColor`](fmlframebkcolor.md) |  |
| [`FmlFrameBkColRGB`](fmlframebkcolrgb.md) |  |
| [`FmlFrameBkColRGB2`](fmlframebkcolrgb2.md) |  |
| [`FmlFrameLnColor`](fmlframelncolor.md) |  |
| [`FmlFrameLnColRGB`](fmlframelncolrgb.md) |  |
| [`FmlFrameLnType`](fmlframelntype.md) |  |
| [`FmlFrameLnWidth`](fmlframelnwidth.md) |  |
| [`FmlFramePt`](fmlframept.md) |  |
| [`FmlTxt`](fmltxt.md) |  |
| [`FmlTxtColor`](fmltxtcolor.md) |  |
| [`FmlTxtColorRGB`](fmltxtcolorrgb.md) |  |
| [`FmlTxtFont`](fmltxtfont.md) |  |
| [`FolderZipName`](folderzipname.md) | Specifies the name of the ZIP archive. |
| [`FolderZipPath`](folderzippath.md) | Specifies the name of the folder. |
| [`ForceVariantType`](forcevarianttype.md) | Specifies whether DIAdem transposes the array with the channel data. DIAdem does not transpose this array by default. |
| [`ForceVirStorage`](forcevirstorage.md) | Specifies whether DIAdem moves data to the hard disk. |
| [`FormulaTxt`](formulatxt.md) | Valid names: FormulaTxt, CalculateFormula |
| [`FrequencyPara`](frequencypara.md) | Valid names: FrequencyPara, RainFrequencyTyp |
| [`FrequencyType`](frequencytype.md) | Specifies whether DIAdem calculates the class frequency absolutely or relatively. |
| [`FSAttrType`](fsattrtype.md) | Specifies the file attribute or the folder attribute. |
| [`FSDateTime`](fsdatetime.md) | Specifies date and time in the time format of the operating system. |
| [`FSDateType`](fsdatetype.md) | Specifies whether you change the time of file creation, of the last change, or of the last access. |
| [`FSPreserveUndo`](fspreserveundo.md) | Specifies whether DIAdem moves files and folders into the recycle bin or deletes them irretrievably. The default value is FALSE which specifies that DIAdem deletes the files irrevocably. |
| [`FSProgressbar`](fsprogressbar.md) | Specifies whether the progress bar remains visible during long operations. If you assign the value TRUE to the FSProgressBar variable, DIAdem does not display the progress bar. The default value for the FSProgressBar variable is FALSE . |
| [`FSSourceName`](fssourcename.md) | Specifies the source file or source folder for DIAdem file and folder commands. |
| [`FSTargetName`](fstargetname.md) | Specifies target folders or target files for DIAdem file and folder commands. |
| [`FSTargetPath`](fstargetpath.md) | Specifies target folders for DIAdem file and folder commands. |
| [`FTPConnectionHandle`](ftpconnectionhandle.md) | Specifies the handle for the FTP connection. |
| [`FTPRetry`](ftpretry.md) | Specifies whether DIAdem retries sending lost data packets following a timeout. |
| [`FullScreenMode`](fullscreenmode.md) | Receives the information whether DIAdem displays in the full-screen mode or in the standard size. This variable is read only. To switch the full screen mode on or off, use the WndShow command. |
| [`FullSpectrumIntervalLength`](fullspectrumintervallength.md) | Specifies the number of values in an interval. |
| [`FullSpectrumIntervalType`](fullspectrumintervaltype.md) | Specifies the data amount of the calculation. |
| [`FullSpectrumNoOfIntervals`](fullspectrumnoofintervals.md) | Specifies the number of intervals. |
| [`FullSpectrumWndCorrectType`](fullspectrumwndcorrecttype.md) | Specifies whether and how DIAdem corrects the damping effect of the window function on the amplitude. |
| [`FullSpectrumWndFct`](fullspectrumwndfct.md) | Specifies the window function. |
| [`FullValueEquidistantCheck`](fullvalueequidistantcheck.md) | Specifies if DIAdem checks whether all values are equidistant or if only a sample is equidistant. |
| [`G1`](g1.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G10`](g10.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G2`](g2.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G3`](g3.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G4`](g4.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G5`](g5.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G6`](g6.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G7`](g7.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G8`](g8.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`G9`](g9.md) | Specifies the contents of the Dynamic enumeration list type single-value auxiliary variable. |
| [`GaussFitAlgorithm`](gaussfitalgorithm.md) | Specifies the algorithm for Gaussian curve fitting. |
| [`GaussFitAmplitude`](gaussfitamplitude.md) | Receives the amplitude of the Gaussian curve fitting. |
| [`GaussFitCenter`](gaussfitcenter.md) | Receives the center of the Gaussian curve fitting. |
| [`GaussFitClipCopy`](gaussfitclipcopy.md) | Specifies whether DIAdem transfers the results of a Gaussian curve fit to the clipboard. |
| [`GaussFitClipValue`](gaussfitclipvalue.md) | Specifies whether DIAdem transfers the results of a Gaussian curve fit to the clipboard as a value or as a variable reference. |
| [`GaussFitFctStr`](gaussfitfctstr.md) | Receives the setup function used by a Gaussian curve fit. |
| [`GaussFitInitCoef`](gaussfitinitcoef.md) | Specifies the start values for the amplitude, the center, and the standard deviation of the Gaussian curve fitting. |
| [`GaussFitResidue`](gaussfitresidue.md) | Receives the residue or the weighted mean error of a Gaussian curve fitting. If you select the Least absolute residual algorithm, the variable receives the absolute error of the weighted mean. If you use other algorithms, the variable does not receive an absolute value. |
| [`GaussFitStdDev`](gaussfitstddev.md) | Receives the standard deviation of the Gaussian curve fitting. |
| [`GaussFitTolerance`](gaussfittolerance.md) | Specifies the tolerance that specifies when to end the iterative fit of the amplitude, the center, and the standard deviation in the bisquare method for a Gaussian curve fitting. If the relative difference of the residual undershoots the tolerance in two successive cycles, the curve fitting stops. If the tolerance is 0, DIAdem sets the tolerance to 0.0001. |
| [`GaussFitWeighted`](gaussfitweighted.md) | Specifies whether DIAdem weights the y-values in a Gaussian curve fitting. |
| [`GenImplicit`](genimplicit.md) | Specifies whether DIAdem generates the channel implicitly. |
| [`GenLSFitAlgorithm`](genlsfitalgorithm.md) | Specifies the algorithm for the general LS linear fitting. |
| [`GenLSFitCovariance`](genlsfitcovariance.md) | Specifies whether DIAdem generates the covariance matrix for a general LS linear fitting. |
| [`GenLSFitMSE`](genlsfitmse.md) | Receives the mean squared error of a general LS linear fitting. |
| [`GenLSFitWeighted`](genlsfitweighted.md) | Specifies whether DIAdem weights the y-values of the general LS linear fitting. |
| [`GenSignalAmplitude`](gensignalamplitude.md) | Specifies the amplitude of the generated channel. |
| [`GenSignalDutyCycle`](gensignaldutycycle.md) | Specifies the symmetry of the generated channel. The value range of the clock ratio is between 0 and 100%. A symmetric signal form has a clock ratio of 50%. |
| [`GenSignalFrequency`](gensignalfrequency.md) | Specifies the frequency of the generated channel in Hertz. |
| [`GenSignalFunction`](gensignalfunction.md) | Specifies the signal form of the generated signal. |
| [`GenSignalNoOfValues`](gensignalnoofvalues.md) | Specifies the number of values in the generated channel. |
| [`GenSignalOffset`](gensignaloffset.md) | Specifies the amplitude offset of the generated channel. |
| [`GenSignalPhaseShift`](gensignalphaseshift.md) | Specifies the phase offset of the generated signals as a percentage of a period. |
| [`GenSignalSamplingRate`](gensignalsamplingrate.md) | Specifies the sampling rate of the generated channel in Hertz, and thus the number of values to be generated for each period. |
| [`GenSignalTimeUnit`](gensignaltimeunit.md) | Specifies the unit of the time values of the generated signal. |
| [`GenSignalUnit`](gensignalunit.md) | Specifies the unit of the amplitude values of the generated channel. |
| [`GenTimeMode`](gentimemode.md) | Specifies whether the last time value or the number of values limits the time channel. |
| [`GenTimeNo`](gentimeno.md) | Specifies the number of values in the new time channel. |
| [`GenTimeStep`](gentimestep.md) | Specifies the step width. |
| [`GenTimeUnit`](gentimeunit.md) | Specifies the time unit for the step width. |
| [`GenTimeXBeg`](gentimexbeg.md) | Specifies the first value in a new time channel. |
| [`GenTimeXEnd`](gentimexend.md) | Specifies the last value in a new time channel. |
| [`GenXBegin`](genxbegin.md) | Specifies the first value in a new data channel. |
| [`GenXEnd`](genxend.md) | Specifies the last value in a new data channel. |
| [`GenXType`](genxtype.md) | Specifies the channel generation mode. |
| [`GenXUnitPreset`](genxunitpreset.md) | Specifies the unit in which DIAdem generates the numeric channel. By default DIAdem does not use a unit. |
| [`GHdASCIIPtr`](ghdasciiptr.md) | If you select the ASCII data type and the Block storage mode, this item specifies which value in each line belongs to a channel. |
| [`GHdChnComment`](ghdchncomment.md) | Specifies a comment for all the channels to be read in, when the channel properties are generated. |
| [`GHdChnFile`](ghdchnfile.md) | Specifies the name and the extension of the ASCII block file that contains the data to be read. |
| [`GHdChnIdx`](ghdchnidx.md) | Specifies the first value in the data file to be read in. |
| [`GHdChnLength`](ghdchnlength.md) | Specifies the maximum number of values per channel. The default value of the GHdChnLength variable is 0 . |
| [`GHdChnMode`](ghdchnmode.md) | Specifies the data type of the data to read in. |
| [`GHdChnName`](ghdchnname.md) | Specifies the name suggestion for a channel in the Data Portal. |
| [`GHdChnNo`](ghdchnno.md) | Specifies the number of channel properties to generate. |
| [`GHdChnType`](ghdchntype.md) | Specifies the data type of the data channel to be generated. |
| [`GHdDecChar`](ghddecchar.md) | Specifies the decimal symbol used in the data file when DIAdem imports ASCII block data. |
| [`GHdDispFormat`](ghddispformat.md) | Specifies the display format of the channel values. The default value of the GHdDispFormat variable is Numeric . |
| [`GHdExChar`](ghdexchar.md) | When DIAdem imports ASCII block data, this variable specifies the exponential character that is used in the data file. |
| [`GHdOffs`](ghdoffs.md) | Specifies the distance between two successive values in a data channel. |
| [`GHdSaveType`](ghdsavetype.md) | Specifies whether DIAdem saves data files channelwise or blockwise. |
| [`GHdSep`](ghdsep.md) | Specifies the separator to blockwise save a DAT file in the ASCII format. |
| [`GHdStartVal`](ghdstartval.md) | Specifies the first value of implicit data channels and the offset of explicit data channels. |
| [`GHdStep`](ghdstep.md) | Specifies the difference between two successive values. |
| [`GHdTimeChnNo`](ghdtimechnno.md) | Specifies the number of the time channel in the ASCII data when DAT file properties are generated. |
| [`Gif`](gif.md) | Specifies the number of registered DLLs. |
| [`GlobChnLength`](globchnlength.md) | Specifies the maximum channel length. |
| [`GlobUsedChn`](globusedchn.md) | Specifies the number of channels in the Data Portal. |
| [`GPIFileDlgState`](gpifiledlgstate.md) |  |
| [`GPIFileDriver`](gpifiledriver.md) | Specifies the name of the GPI DLL for an external file. |
| [`GPIFileDrvExt`](gpifiledrvext.md) | Specifies the filename extension of the registered GPI file driver. |
| [`GPIFileDrvFlags`](gpifiledrvflags.md) | Specifies the functions complexity of the registered GPI file driver. |
| [`GPIFileDrvLibNr`](gpifiledrvlibnr.md) | Specifies the library index for a registered GPI-DLL. |
| [`GPIFileDrvName`](gpifiledrvname.md) | Specifies the name of the registered DLLs. |
| [`GPIFileDrvType`](gpifiledrvtype.md) | Specifies the file type for a registered GPI-DLL. |
| [`GPIGetDrvLibNr`](gpigetdrvlibnr.md) | Specifies the index of a registered GPI-DLL. |
| [`GPILibComment`](gpilibcomment.md) | Specifies the comment of a registered GPI-DLL. |
| [`GPILibCompAdr`](gpilibcompadr.md) | Specifies the address of the company that created the registered GPI-DLL. |
| [`GPILibCompany`](gpilibcompany.md) | Specifies the name of the company that created the registered GPI-DLL. |
| [`GPILibCompPhone`](gpilibcompphone.md) | Specifies the telephone number of the company that created the registered GPI-DLL. |
| [`GPILibCompVers`](gpilibcompvers.md) | Specifies the version number of a registered GPI-DLL. |
| [`GPILibCopyright`](gpilibcopyright.md) | Specifies the copyright of a registered GPI-DLL. |
| [`GPILibDLLName`](gpilibdllname.md) | Specifies the name of a registered GPI-DLL. |
| [`GPILibExtents`](gpilibextents.md) | Specifies the number of GPI-DLLs registered in DIAdem. |
| [`GPILibName`](gpilibname.md) | Specifies the name of a registered GPI-DLL. |
| [`GPILibNumber`](gpilibnumber.md) | Specifies the number of registered GPI-DLLs. |
| [`GPILibState`](gpilibstate.md) | Specifies the status of a GPI DLL. |
| [`GPILibVersion`](gpilibversion.md) | Specifies the version number of a registered GPI-DLL. |
| [`GPIVarName`](gpivarname.md) | Contains the registered GPI commands and variables. |
| [`GPIVarNumber`](gpivarnumber.md) | Specifies the number of all the GPI commands and variables registered in DIAdem. |
| [`GPIVarOv0Str`](gpivarov0str.md) | Specifies the properties of a registered GPI variable. |
| [`GPIVarType`](gpivartype.md) | Specifies the type of a registered GPI variable. |
| [`GraphDrvLibr`](graphdrvlibr.md) |  |
| [`GraphDrvUser`](graphdrvuser.md) | Valid names: GraphDrvUser, GraphDrv |
| [`GraphObjName`](graphobjname.md) | Valid names: GraphObjName, CurrObjName, CurrMainObjectName |
| [`GraphObjNewName`](graphobjnewname.md) | Valid names: GraphObjNewName, CurrCurveObjectName |
| [`GroupChnCount`](groupchncount.md) |  |
| [`GroupCount`](groupcount.md) | Specifies the number of channel groups in the Data Portal. You also can use the object-oriented interface to access internal data. Use ChannelGroups . Count from the script interface for internal data to realize the functionality of the GroupCount variable. |
| [`GroupCreateName`](groupcreatename.md) |  |
| [`GroupDefaultGet`](groupdefaultget.md) |  |
| [`GroupDescript`](groupdescript.md) |  |
| [`GroupName`](groupname.md) |  |
| [`GroupPropCount`](grouppropcount.md) |  |
| [`GV`](gv.md) | Specifies the contents of the Dynamic enumeration list type vector-auxiliary variable. |
| [`HCD15`](hcd15.md) | Specifies whether DIAdem calculates the 15 ms value. |
| [`HCD15MeanAcc`](hcd15meanacc.md) | Receives the mean value for the neck acceleration from the HCD calculation between T1 and T2 for 15 ms. |
| [`HCD15T1`](hcd15t1.md) | Receives the T1 values from the HCD calculation for 15 ms. |
| [`HCD15T2`](hcd15t2.md) | Receives the T2 values from the HCD calculation for 15 ms. |
| [`HCD15Value`](hcd15value.md) | Receives the HCD value for 15 ms. |
| [`HCD36`](hcd36.md) | Specifies whether DIAdem calculates the 36 ms value. |
| [`HCD36MeanAcc`](hcd36meanacc.md) | Receives the mean value for the neck acceleration from the HCD calculation between T1 and T2 for 36 ms. |
| [`HCD36T1`](hcd36t1.md) | Receives the T1 values from the HCD calculation for 36 ms. |
| [`HCD36T2`](hcd36t2.md) | Receives the T2 values from the HCD calculation for 36 ms. |
| [`HCD36Value`](hcd36value.md) | Receives the HCD value for 36 ms. |
| [`HCDClipCopy`](hcdclipcopy.md) | Specifies whether DIAdem transfers the HCD results to the clipboard. |
| [`HCDClipValue`](hcdclipvalue.md) | Specifies whether DIAdem transfers the HCD results to the clipboard as values or as variable references. |
| [`HCDMeanAcc`](hcdmeanacc.md) | Receives the mean value for the neck acceleration of the HCD calculation between T1 and T2 for an unlimited period. |
| [`HCDRes`](hcdres.md) | Receives the result matrix of the HCD calculation. |
| [`HCDT1`](hcdt1.md) | Receives the T1 values from the HCD calculation for an unlimited period. |
| [`HCDT2`](hcdt2.md) | Receives the T2 values of the HCD calculation for an unlimited period. |
| [`HCDUser`](hcduser.md) | Specifies the width of the window in milliseconds when calculating the HCD value. |
| [`HCDUserDef`](hcduserdef.md) | Specifies whether DIAdem calculates the HCD value with adjustable window width. |
| [`HCDUserMeanAcc`](hcdusermeanacc.md) | Receives the mean value of the neck acceleration of the HCD calculation between T1 and T2 for the value specified in ms. |
| [`HCDUserT1`](hcdusert1.md) | Receives the T1 values from the HCD calculation for the value specified in ms. |
| [`HCDUserT2`](hcdusert2.md) | Receives the T2 values from the HCD calculation for the value specified in ms. |
| [`HCDUserValue`](hcduservalue.md) | Receives the HCD value for the value specified in ms. |
| [`HCDValue`](hcdvalue.md) | Receives the HCD value for an unlimited period of time. |
| [`HCDVar`](hcdvar.md) | Specifies whether DIAdem calculates the HCD value. |
| [`HCDVersion`](hcdversion.md) | Receives the version number of the HCD calculation routine. |
| [`HdChnArg1`](hdchnarg1.md) | Uses the channel name or the channel number to specify a channel. |
| [`HdChnArg2`](hdchnarg2.md) | Uses the channel name or the channel number to specify a target channel. |
| [`HdFile`](hdfile.md) | Specifies the name of a data set header file in the DAT format. |
| [`HdFileSave`](hdfilesave.md) | When DIAdem imports ASCII block data, this variable specifies whether to save the channel properties. |
| [`HeaderDel`](headerdel.md) | Specifies whether DIAdem deletes the data set comments. The default value is FALSE , which specifies that DIAdem does not delete the data set comments. |
| [`HIC15`](hic15.md) | Specifies whether DIAdem calculates the 15 ms value. |
| [`HIC15MeanAcc`](hic15meanacc.md) | Receives the mean value for the head acceleration from the HIC calculation between T1 and T2 for 15 ms. |
| [`HIC15T1`](hic15t1.md) | Receives the T1 values of the HIC calculation for 15 ms. |
| [`HIC15T2`](hic15t2.md) | Receives the T2 values of the HIC calculation for 15 ms. |
| [`HIC15Value`](hic15value.md) | Receives the HIC value for 15 ms. |
| [`HIC36`](hic36.md) | Specifies whether DIAdem calculates the 36 ms value. |
| [`HIC36MeanAcc`](hic36meanacc.md) | Receives the mean value for the head acceleration from the HIC calculation between T1 and T2 for 36 ms. |
| [`HIC36T1`](hic36t1.md) | Receives the T1 values of the HIC calculation for 36 ms. |
| [`HIC36T2`](hic36t2.md) | Receives the T2 values of the HIC calculation for 36 ms. |
| [`HIC36Value`](hic36value.md) | Receives the HIC value for 36 ms. |
| [`HICClipCopy`](hicclipcopy.md) | Specifies whether DIAdem transfers the HIC results to the clipboard. |
| [`HICClipValue`](hicclipvalue.md) | Specifies whether DIAdem transfers the HIC results to the clipboard as values or as variable references. |
| [`HICd`](hicd.md) | Specifies whether DIAdem calculates the HIC(d) value. The default value is FALSE which means that DIAdem does not calculate the HIC(d) value. |
| [`HICdMeanAcc`](hicdmeanacc.md) | Receives the mean value for the head acceleration of the HIC(d) calculation between T1 and T2 for 15 ms. |
| [`HICdT1`](hicdt1.md) | Receives the T1 values of the HIC(d) calculation. |
| [`HICdT2`](hicdt2.md) | Receives the T1 values of the HIC(d) calculation. |
| [`HICdValue`](hicdvalue.md) | Receives the HIC(d) values. |
| [`HICMeanAcc`](hicmeanacc.md) | Receives the mean value for the head acceleration of the HIC calculation between T1 and T2 for an unlimited period. |
| [`HICRangeNo`](hicrangeno.md) | Specifies the number of columns of an HIC result matrix. |
| [`HICRes`](hicres.md) | Receives the result matrix of an HIC calculation. |
| [`HICResNo`](hicresno.md) | Specifies the number of rows of an HIC result matrix. |
| [`HICT1`](hict1.md) | Receives the T1 values from the HIC calculation for an unlimited period. |
| [`HICT2`](hict2.md) | Receives the T2 values of the HIC calculation for an unlimited period. |
| [`HICUser`](hicuser.md) | Specifies the width of the window in milliseconds when calculating the HIC value. |
| [`HICUserDef`](hicuserdef.md) | Specifies whether DIAdem calculates the HIC value with adjustable window width. |
| [`HICUserMeanAcc`](hicusermeanacc.md) | Receives the mean value of the head acceleration of the HIC calculation between T1 and T2 for the value specified in ms. |
| [`HICUserT1`](hicusert1.md) | Receives the T1 values from the HIC calculation for the value specified in ms. |
| [`HICUserT2`](hicusert2.md) | Receives the T2 values from the HIC calculation for the value specified in ms. |
| [`HICUserValue`](hicuservalue.md) | Receives the mean value from the head acceleration between T1 and T2 for the value specified in ms. |
| [`HICValue`](hicvalue.md) | Receives the HIC value for an unlimited period. |
| [`HICVar`](hicvar.md) | Specifies whether DIAdem calculates the HIC value. |
| [`HICVersion`](hicversion.md) | Receives the version number of the HIC calculation routine. |
| [`HPC15`](hpc15.md) | Specifies whether DIAdem calculates the 15 ms value. |
| [`HPC15MeanAcc`](hpc15meanacc.md) | Receives the mean value for the head acceleration of the HPC calculation between T1 and T2 for 15 ms. |
| [`HPC15T1`](hpc15t1.md) | Receives the T1 values of the HPC calculation for 15 ms. |
| [`HPC15T2`](hpc15t2.md) | Receives the T2 values of the HPC calculation for 15 ms. |
| [`HPC15Value`](hpc15value.md) | Receives the HPC value for 15 ms. |
| [`HPC36`](hpc36.md) | Specifies whether DIAdem calculates the 36 ms value. |
| [`HPC36MeanAcc`](hpc36meanacc.md) | Receives the mean value for the head acceleration of the HPC calculation between T1 and T2 for 36 ms. |
| [`HPC36T1`](hpc36t1.md) | Receives the T1 values of the HPC calculation for 36 ms. |
| [`HPC36T2`](hpc36t2.md) | Receives the T2 values of the HPC calculation for 36 ms. |
| [`HPC36Value`](hpc36value.md) | Receives the HPC value for 36 ms. |
| [`HPCClipCopy`](hpcclipcopy.md) | Specifies whether DIAdem transfers the HPC results to the clipboard. |
| [`HPCClipValue`](hpcclipvalue.md) | Specifies whether DIAdem transfers the HPC results to the clipboard as values or as variable references. |
| [`HPCMeanAcc`](hpcmeanacc.md) | Receives the mean value for the head acceleration of the HIC calculation between T1 and T2 for an unlimited period. |
| [`HPCRes`](hpcres.md) | Receives the result matrix of the HIC calculation. |
| [`HPCT1`](hpct1.md) | Receives the T1 values from the HIC calculation for an unlimited period. |
| [`HPCT2`](hpct2.md) | Receives the T2 values of the HIC calculation for an unlimited period. |
| [`HPCUser`](hpcuser.md) | Specifies the width of the window in milliseconds when calculating the HPC value. |
| [`HPCUserDef`](hpcuserdef.md) | Specifies whether DIAdem calculates the HPC value with adjustable window width. |
| [`HPCUserMeanAcc`](hpcusermeanacc.md) | Receives the mean value of the head acceleration of the HPC calculation between T1 and T2 for the value specified in ms. |
| [`HPCUserT1`](hpcusert1.md) | Receives the T1 values of the HPC calculation for the value specified in ms. |
| [`HPCUserT2`](hpcusert2.md) | Receives the T2 values of the HPC calculation for the value specified in ms. |
| [`HPCUserValue`](hpcuservalue.md) | Receives the HPC value for the value specified in ms. |
| [`HPCValue`](hpcvalue.md) | Receives the HPC value for an unlimited period. |
| [`HPCVar`](hpcvar.md) | Specifies whether DIAdem calculates the HPC value. |
| [`HPCVersion`](hpcversion.md) | Receives the version number of the HPC calculation routine. |
| [`HullFactor`](hullfactor.md) | In a non-convex hull calculation, this specifies the factor by which the new edge can be longer than the old edge. |
| [`HullTol`](hulltol.md) | When DIAdem calculates a non-convex hull, this variable specifies the maximum length of any edge of the hull as a percentage of the cross section of the set of points. |
| [`HullType`](hulltype.md) | Specifies whether DIAdem calculates the convex or the non-convex hull. |
| [`Hysteresis`](hysteresis.md) | Specifies the hysteresis as a percentage of the average class width. |
| [`IconTargetPath`](icontargetpath.md) | Specifies the absolute path where DIAdem saves the generated ICO file. If the path entry is blank, DIAdem saves the ICO file in the source path. |
| [`IDay`](iday.md) | Specifies the day. |
| [`IFFTHilbert`](iffthilbert.md) | Specifies the phase shift for inverse fast Fourier transform. The default value of the IFFTHilbert variable is No . |
| [`IgnoreUnknownUnits`](ignoreunknownunits.md) | Specifies whether DIAdem ignores unknown units ( TRUE ) or whether DIAdem outputs an error ( FALSE ). |
| [`IHour`](ihour.md) | Specifies the hour. |
| [`ImageAreaHeight`](imageareaheight.md) | Specifies the height of the rectangular extract, in pixels. |
| [`ImageAreaWidth`](imageareawidth.md) | Specifies the width of the rectangular extract, in pixels. |
| [`ImageAreaX`](imageareax.md) | Specifies the distance between the rectangular section and the left edge, in pixels. |
| [`ImageAreaY`](imageareay.md) | Specifies the distance between the rectangular section and the top edge, in pixels. |
| [`ImageFile`](imagefile.md) | Specifies the name and the path of the graphics file. Supported file types: .bmp, .jpg, .tif, .wmf, .emf, .pcx, .png, and .gif. |
| [`ImageTransparentColor`](imagetransparentcolor.md) | Specifies the RGB value of the transparent color. If the value is -1, DIAdem does not use transparent color. |
| [`IMicrosecond`](imicrosecond.md) | Specifies the microsecond. |
| [`IMillisecond`](imillisecond.md) | Specifies the millisecond. |
| [`IMinute`](iminute.md) | Specifies the minute. |
| [`IMonth`](imonth.md) | Specifies the month. |
| [`ImplicitChk`](implicitchk.md) | Specifies whether DIAdem checks implicit channels when saving a data set. |
| [`ImportAction`](importaction.md) | Specifies how DIAdem imports data into the Data Portal. The default value of the ImportAction variable is Load . |
| [`ImportParameterSet`](importparameterset.md) | Specifies how DIAdem imports data into the Data Portal. Use the ImportParameter object for the ImportParameterSet parameter. You can also use one of the following script terms as an alternative. If the script term contains "\|ChnXYRelation" , DIAdem maintains the reference to the x-channel for xy-channels . |
| [`ImportSelection`](importselection.md) | Specifies which data channels to load from a data file. |
| [`INanosecond`](inanosecond.md) | Specifies the nanosecond. |
| [`IncludeHdLoad`](includehdload.md) | Specifies whether DIAdem transfers the data set properties into the Data Portal. |
| [`InputPath`](inputpath.md) | Valid names: InputPath, DlgInputPath |
| [`InstallationKeyword`](installationkeyword.md) | Specifies the type of installation information that you request. |
| [`IntChk`](intchk.md) | Specifies whether DIAdem checks integer channels when saving a data set. |
| [`IntegrationConstant`](integrationconstant.md) | Specifies the constant, which DIAdem adds to the integral after the integration. |
| [`IntegrationConstantManual`](integrationconstantmanual.md) | Specifies whether DIAdem uses an integration constant for the trapezoidal rule. Do not enable this option if you want to continue to calculate with the method valid up to version 2012. The integration constant is always used with the Simpson rule. |
| [`IntegrationFinalValue`](integrationfinalvalue.md) | Specifies the integration end value according to the Simpson rule. |
| [`IntegrationMethod`](integrationmethod.md) | Specifies the integration method. |
| [`InterActionNo`](interactionno.md) | Specifies the number of active interactions. |
| [`InteractionText`](interactiontext.md) | Specifies the text that DIAdem displays in a non-modal dialog box when the interaction is enabled. By default the InteractionText variable contains an empty text. |
| [`IntervalMethod`](intervalmethod.md) | Specifies whether DIAdem divides a channel into a specific number of intervals or whether you enter the number of values per interval. |
| [`IntervalType`](intervaltype.md) | Specifies the interval type. |
| [`IntervalValue`](intervalvalue.md) | Specifies the number of intervals or the interval width, depending on which value IntervalMethod contains. |
| [`IntroDlgShow`](introdlgshow.md) | Specifies whether DIAdem displays the introduction screen when the program starts. |
| [`IsAvailLabVIEW`](isavaillabview.md) | Specifies whether LabVIEW is installed on your computer. |
| [`IsAvailMicrosoftPDFPrinter`](isavailmicrosoftpdfprinter.md) | Specifies whether a Microsoft PDF printer is installed on your computer. |
| [`IsAvailOPCUA`](isavailopcua.md) | Specifies whether the OPC-UA driver is part of a DIAdem installation. |
| [`IsAvailPython`](isavailpython.md) | Determines whether a Python version usable by DIAdem is installed on the computer. |
| [`ISecond`](isecond.md) | Specifies the second. |
| [`IsExportFilter`](isexportfilter.md) | Specifies which file filter DIAdem checks. If you assign the value TRUE to the IsExportFilter variable, or if you do not specify the variable, DIAdem checks for the import filter otherwise for the export filter. |
| [`IsMasterlayout`](ismasterlayout.md) |  |
| [`ItemInfoID`](iteminfoid.md) | Receives the variable or command number. |
| [`ItemInfoMaxCol`](iteminfomaxcol.md) | Receives the maximum second index of a matrix variable. |
| [`ItemInfoMaxCVal`](iteminfomaxcval.md) | Receives the maximum second index of a matrix variable as text or as a variable reference. |
| [`ItemInfoMaxRow`](iteminfomaxrow.md) | Receives the maximum first index of a vector variable or of a matrix variable. |
| [`ItemInfoMaxRVal`](iteminfomaxrval.md) | Receives the maximum first index of a vector variable or of a matrix variable as text or as a variable reference. |
| [`ItemInfoMinIndex`](iteminfominindex.md) | Receives the minimum index value of a vector variable or of a matrix variable. |
| [`ItemInfoParam`](iteminfoparam.md) | Receives the parameter set of a command or the value range of a variable. |
| [`ItemInfoRange`](iteminforange.md) | Receives the value range of a variable. |
| [`ItemInfoType`](iteminfotype.md) | Receives the variable or command type. |
| [`ItemInfoVarDim`](iteminfovardim.md) | Receives notification whether a variable is a scalar, a vector, or a matrix. |
| [`ItemInfoVarType`](iteminfovartype.md) | Receives the variable or command type. |
| [`ItemName`](itemname.md) | Specifies the name of a DIAdem variable or of a DIAdem command. |
| [`IYear`](iyear.md) | Specifies the year. |
| [`KeepAssignmentProperties`](keepassignmentproperties.md) | Specifies that the assignment channel remains when DIAdem writes the assignments into a new text channel. The default value of the variable is TRUE , so that DIAdem does not delete the assignments in the assignment channel. |
| [`KeepWfProperties`](keepwfproperties.md) | Specifies whether DIAdem maintains the waveform properties during this operation. The default value is FALSE and specifies that DIAdem does not maintain the waveform properties. |
| [`KFiltAverageTime`](kfiltaveragetime.md) | Specifies the time constant for mean calculations, in seconds. |
| [`KFiltNorm`](kfiltnorm.md) | Specifies whether DIAdem normalizes the k-value calculation. |
| [`KFiltOscillation`](kfiltoscillation.md) | Specifies whether DIAdem calculates the weighted oscillation severity. |
| [`KFiltRedFactor`](kfiltredfactor.md) | Specifies that DIAdem reduces the result values to each nth k-value, starting at the first result value. |
| [`KFiltType`](kfilttype.md) | Specifies the frequency weighting filter for time-related body and hand-arm vibrations. |
| [`KFiltValMax`](kfiltvalmax.md) | Receives the highest evaluated vibration severity of a k-value analysis. |
| [`KTHFMax`](kthfmax.md) | Receives the maximum value of the forces impacting the hips and thighs, in kilo newton. |
| [`KTHImpulse`](kthimpulse.md) | Receives the impulse of KTHt0 after KTHt1, in Newton seconds. |
| [`KTHRating`](kthrating.md) | Receives the evaluation of the KTH calculation through the maximum value and the impulse. |
| [`KTHt0`](ktht0.md) | Receives the time span until the last zero crossing before reaching the maximum value, in milliseconds. |
| [`KTHt1`](ktht1.md) | Receives the time span as far as the falling slope after reaching the maximum value, in milliseconds. |
| [`KTHVersion`](kthversion.md) | Receives the version number of the KTH calculation routine. |
| [`L1`](l1.md) | Specifies a freely usable longinteger variable. |
| [`L10`](l10.md) | Specifies a freely usable longinteger variable. |
| [`L11`](l11.md) | Specifies a freely usable longinteger variable. |
| [`L12`](l12.md) | Specifies a freely usable longinteger variable. |
| [`L13`](l13.md) | Specifies a freely usable longinteger variable. |
| [`L14`](l14.md) | Specifies a freely usable longinteger variable. |
| [`L15`](l15.md) | Specifies a freely usable longinteger variable. |
| [`L16`](l16.md) | Specifies a freely usable longinteger variable. |
| [`L17`](l17.md) | Specifies a freely usable longinteger variable. |
| [`L18`](l18.md) | Specifies a freely usable longinteger variable. |
| [`L19`](l19.md) | Specifies a freely usable longinteger variable. |
| [`L2`](l2.md) | Specifies a freely usable longinteger variable. |
| [`L20`](l20.md) | Specifies a freely usable longinteger variable. |
| [`L21`](l21.md) | Specifies a freely usable longinteger variable. |
| [`L22`](l22.md) | Specifies a freely usable longinteger variable. |
| [`L23`](l23.md) | Specifies a freely usable longinteger variable. |
| [`L24`](l24.md) | Specifies a freely usable longinteger variable. |
| [`L25`](l25.md) | Specifies a freely usable longinteger variable. |
| [`L26`](l26.md) | Specifies a freely usable longinteger variable. |
| [`L27`](l27.md) | Specifies a freely usable longinteger variable. |
| [`L28`](l28.md) | Specifies a freely usable longinteger variable. |
| [`L29`](l29.md) | Specifies a freely usable longinteger variable. |
| [`L3`](l3.md) | Specifies a freely usable longinteger variable. |
| [`L30`](l30.md) | Specifies a freely usable longinteger variable. |
| [`L31`](l31.md) | Specifies a freely usable longinteger variable. |
| [`L32`](l32.md) | Specifies a freely usable longinteger variable. |
| [`L4`](l4.md) | Specifies a freely usable longinteger variable. |
| [`L5`](l5.md) | Specifies a freely usable longinteger variable. |
| [`L6`](l6.md) | Specifies a freely usable longinteger variable. |
| [`L7`](l7.md) | Specifies a freely usable longinteger variable. |
| [`L8`](l8.md) | Specifies a freely usable longinteger variable. |
| [`L9`](l9.md) | Specifies a freely usable longinteger variable. |
| [`LabVIEWPath`](labviewpath.md) | Specifies the program path of the installed LabVIEW version. |
| [`LastErrorFile`](lasterrorfile.md) |  |
| [`LastErrorIs`](lasterroris.md) | Valid names: LastErrorIs, LastErrorVReset |
| [`LastErrorNo`](lasterrorno.md) |  |
| [`LastErrorPart`](lasterrorpart.md) |  |
| [`LastErrorText`](lasterrortext.md) |  |
| [`Latitude1`](latitude1.md) | Specifies the latitude of the first coordinate. |
| [`Latitude2`](latitude2.md) | Specifies the latitude of the second coordinate. |
| [`LayoutLibrPath`](layoutlibrpath.md) | Specifies the current library path for VIEW layouts and for REPORT layouts. |
| [`LayoutReadPath`](layoutreadpath.md) | Specifies the current read path for VIEW layouts and for REPORT layouts. |
| [`LayoutWritePath`](layoutwritepath.md) | Specifies the current write path for VIEW layouts and for REPORT layouts. |
| [`LegColNoMax`](legcolnomax.md) | Specifies the maximum number of legend columns. |
| [`LengthUnit`](lengthunit.md) | Specifies which unit DIAdem uses. |
| [`LineWidthLst`](linewidthlst.md) | Specifies a list with line widths. |
| [`LoadedElementList`](loadedelementlist.md) | Specifies the ElementList object , which contains the loaded data elements. |
| [`LocalWorker`](localworker.md) | The LocalWorker object provides access to the worker within the parallel processing process. A Worker DIAdem uses the LocalWorker object to exchange data with the master program. |
| [`LogfileEditName`](logfileeditname.md) | Specifies the text editor for displaying and editing a logfile. You must include the editor path if the editor is not in the Windows folder. |
| [`LogfileExtent`](logfileextent.md) | Specifies the type of messages that DIAdem records in a logfile. |
| [`LogfileReset`](logfilereset.md) | Specifies the maximum number of messages that DIAdem records in a logfile. When the logfile exceeds this number, DIAdem deletes all messages in the logfile. |
| [`Longitude1`](longitude1.md) | Specifies the longitude of the first coordinate. |
| [`Longitude2`](longitude2.md) | Specifies the longitude of the second coordinate. |
| [`LoopLength`](looplength.md) | Specifies the percentage of the progress bar in the status bar. Valid values range between 1 and 100. |
| [`LV1`](lv1.md) | Specifies a freely usable longinteger vector. |
| [`LV2`](lv2.md) | Specifies a freely usable longinteger vector. |
| [`LV3`](lv3.md) | Specifies a freely usable longinteger vector. |
| [`LVRuntime`](lvruntime.md) | Specifies the LVRuntime object that enables access to LabVIEW. Use the LVRuntime object to load and to execute VIs. |
| [`LVTemplatePath`](lvtemplatepath.md) | Specifies the path of the VI which LabVIEW opens after the program is launched out of DIAdem. |
| [`LVTemplateVI`](lvtemplatevi.md) | Specifies the VI that LabVIEW opens when you start LabVIEW from DIAdem. |
| [`MainObjectName`](mainobjectname.md) | Specifies the object that contains the curve section. |
| [`MapLinBdryVal`](maplinbdryval.md) | Specifies the constant value for extrapolation with a constant value. |
| [`MapLinExtType`](maplinexttype.md) | Specifies the extrapolation type that DIAdem uses to extend mapping outside the original x-range. |
| [`MapLinFctType`](maplinfcttype.md) | Specifies the type of function that is to be mapped. |
| [`MapLinInnerVal`](maplininnerval.md) | Specifies the value that DIAdem uses in the linear mapping process of spike curves for those values to which DIAdem does not assign an interpolation point. The default value of the MapLinInnerVal variable is 0 . |
| [`MapLinNovInterp`](maplinnovinterp.md) | Specifies whether DIAdem replaces NoValues in the y-values. |
| [`MarkerList`](markerlist.md) | Specifies a list with marker symbols. |
| [`MasterlayoutAUpd`](masterlayoutaupd.md) |  |
| [`MasterlayoutLink`](masterlayoutlink.md) |  |
| [`MasterlayoutPath`](masterlayoutpath.md) |  |
| [`MasterlayoutTime`](masterlayouttime.md) |  |
| [`MatExtCheckPos`](matextcheckpos.md) | Specifies whether DIAdem determines the columns and rows that contain the extreme values. |
| [`MatMatOpType`](matmatoptype.md) | Specifies the matrix operations such as addition, subtraction, division, or multiplication. |
| [`MatMax`](matmax.md) | Receives the maximum value of a matrix. |
| [`MatMaxCol`](matmaxcol.md) | Receives the column number of the maximum value of a matrix. |
| [`MatMaxRow`](matmaxrow.md) | Receives the row number of the maximum value of a matrix. |
| [`MatMin`](matmin.md) | Receives the minimum value of a matrix. |
| [`MatMinCol`](matmincol.md) | Receives the column number of the minimum value of a matrix. |
| [`MatMinRow`](matminrow.md) | Receives the row number of the minimum value of a matrix. |
| [`MatMulType`](matmultype.md) | Specifies whether DIAdem multiplies the matrices componentwise or algebraically. |
| [`MatNormIP`](matnormip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result values from the normalizing. |
| [`MatRelIP`](matrelip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result values of the relativization. |
| [`MatScalIP`](matscalip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result values of the matrix operation. |
| [`MatScalOpType`](matscaloptype.md) | Specifies which operation DIAdem uses. |
| [`MatScalVal`](matscalval.md) | Specifies the scalar value that DIAdem uses to add or to multiply the matrix componentwise. |
| [`MatSortIP`](matsortip.md) | Specifies whether DIAdem overwrites the values of the input channels with the sorting result values. The default value is FALSE which specifies that DIAdem does not overwrite the input channels. |
| [`MatTransIP`](mattransip.md) | Specifies whether DIAdem overwrites the values of the input channels with the transposition result values. The default value is FALSE which specifies that DIAdem does not overwrite the input channels. |
| [`MatVOpType`](matvoptype.md) | Specifies which operation DIAdem uses. |
| [`MaxCurveNo`](maxcurveno.md) |  |
| [`MaxNegFloat`](maxnegfloat.md) | Specifies the maximum negative number that DIAdem processes. |
| [`MaxPosFloat`](maxposfloat.md) | Specifies the maximum positive number that DIAdem processes. |
| [`MaxTime`](maxtime.md) | Receives the time of the maximum value. |
| [`MaxXPage`](maxxpage.md) |  |
| [`MaxYPage`](maxypage.md) |  |
| [`MediaLibrPath`](medialibrpath.md) | Specifies the current library path for media, such as graphics, videos, PDF files, and HTML files. |
| [`MediaReadPath`](mediareadpath.md) | Specifies the current read path for media, such as graphics, videos, PDF files, and HTML files. |
| [`MediaWritePath`](mediawritepath.md) | Specifies the current write path for media, such as graphics, videos, PDF files, and HTML files. |
| [`MenuItemCount`](menuitemcount.md) |  |
| [`MenuItemFct`](menuitemfct.md) |  |
| [`MenuItemPos`](menuitempos.md) |  |
| [`MenuItemTitle`](menuitemtitle.md) |  |
| [`MenuItemType`](menuitemtype.md) |  |
| [`MenusVisible`](menusvisible.md) | Valid names: MenusVisible, ApplicationMenuVisible |
| [`MinMaxVer`](minmaxver.md) | Receives the version number of the MinMax calculation routine. |
| [`MinTime`](mintime.md) | Receives the time of the minimum value. |
| [`MqttUrl`](mqtturl.md) | Specifies the URL of the MQTT broker. The URL can also contain the port. By default, DIAdem uses port 1883 for unencrypted communication and port 8883 for encrypted communication. |
| [`MsgBoxHeight`](msgboxheight.md) | Specifies the height of a message box. |
| [`MsgBoxWidth`](msgboxwidth.md) | Specifies the width of a message box. |
| [`MsgBoxXPos`](msgboxxpos.md) | Specifies the x-position of a message box in relation to the left edge. |
| [`MsgBoxYPos`](msgboxypos.md) | Specifies the y-position of a message box, in relation to the bottom edge. |
| [`MsgButtonText1`](msgbuttontext1.md) | Specifies the label text for the first button in a message box. By default the MsgButtonType parameter of the subsequent command MsgBoxDisp specifies the button labels. |
| [`MsgButtonText2`](msgbuttontext2.md) | Specifies the label text for the second button in a message box. By default the MsgButtonType parameter of the subsequent command MsgBoxDisp specifies the button labels. |
| [`MsgButtonText3`](msgbuttontext3.md) | Specifies the label text for the third button in a message box. By default the MsgButtonType parameter of the subsequent command MsgBoxDisp specifies the button labels. |
| [`MsgButtonType`](msgbuttontype.md) | Specifies the type and number of buttons in a message box. The default value of the MsgButtonType variable is MB_OK . |
| [`MsgNotModal`](msgnotmodal.md) | Specifies whether DIAdem opens a message box modally or non-modally. The default value is FALSE which means that DIAdem opens the message box in modal mode. |
| [`MsgState`](msgstate.md) | Valid names: MsgState, WarningAnswer |
| [`MsgStdButton`](msgstdbutton.md) | Specifies the standard button for a message box. The default value of the MsgStdButton variable is 0 . |
| [`MsgText`](msgtext.md) | Specifies the text of a message. |
| [`MsgTimeOut`](msgtimeout.md) | Specifies how many seconds elapse before DIAdem closes a message box. The default value of the MsgTimeOut variable is 0 . |
| [`MsgType`](msgtype.md) | Specifies the type of a message box. The default value of the MsgType variable is MsgTypeNote . |
| [`MtaBackColor`](mtabackcolor.md) |  |
| [`MtaBackRGB`](mtabackrgb.md) |  |
| [`MtaClip`](mtaclip.md) |  |
| [`MtaEmbedded`](mtaembedded.md) |  |
| [`MtaFileName`](mtafilename.md) | Valid names: MtaFileName, MetaFileName |
| [`MtaHeight`](mtaheight.md) |  |
| [`MtaPosX`](mtaposx.md) |  |
| [`MtaPosY`](mtaposy.md) |  |
| [`MtaRatio`](mtaratio.md) |  |
| [`MtaRatioAdapt`](mtaratioadapt.md) |  |
| [`MtaRelPos`](mtarelpos.md) |  |
| [`MtaWidth`](mtawidth.md) |  |
| [`MultipleSortExtCaseSensitive`](multiplesortextcasesensitive.md) | Specifies whether and how DIAdem sorts text case-sensitively. |
| [`MultipleSortExtIP`](multiplesortextip.md) | Specifies that DIAdem stores the results in the original channels. |
| [`MultipleSortExtOrder`](multiplesortextorder.md) | Specifies whether DIAdem sorts values and text in ascending or descending order. DIAdem sorts texts according to the ASCII table. |
| [`NAVIGATOR`](navigator.md) | Specifies the object that provides access to the subobjects, methods, and properties in DIAdem NAVIGATOR. |
| [`NaviInitMode`](naviinitmode.md) | Specifies whether DIAdem opens a DataFinder or a data store when DIAdem NAVIGATOR starts. |
| [`NaviInitStore`](naviinitstore.md) | Specifies the data storage that DIAdem opens when the DIAdem NAVIGATOR panel starts. |
| [`NICForceType`](nicforcetype.md) | Specifies whether the forces are axial tensile forces or shear forces. |
| [`NICRearMax`](nicrearmax.md) | Receives the NIC maximum value, in meters per square second. |
| [`NICRearTime`](nicreartime.md) | Receives the time for the NIC maximum value, in seconds. |
| [`NICRearVersion`](nicrearversion.md) | Receives the version number of the Neck Injury Criterion Rear Impact calculation routine. |
| [`NICVersion`](nicversion.md) | Receives the version number of the FFC calculation routine. |
| [`NijAll`](nijall.md) | Specifies that DIAdem calculates all Nij values. |
| [`NijFzc`](nijfzc.md) | Specifies the critical compression force in newtons. |
| [`NijFzcNCE`](nijfzcnce.md) |  |
| [`NijFzcNCF`](nijfzcncf.md) |  |
| [`NijFzcNTF`](nijfzcntf.md) |  |
| [`NijMax`](nijmax.md) | Receives the maximum value of the NIJ calculation. |
| [`NijMaxCompression`](nijmaxcompression.md) | Specifies the critical bending moment in newton meters in the negative y-direction. |
| [`NijMaxExtension`](nijmaxextension.md) | Specifies the critical bending moment in newton meters in the positive y-direction. |
| [`NijMaxFlexion`](nijmaxflexion.md) | Specifies the critical compression force in newtons in the positive z-direction. |
| [`NijMaxTension`](nijmaxtension.md) | Specifies the critical tensile force in newtons in the negative z-direction. |
| [`NijMyc`](nijmyc.md) | Specifies the critical bending moment in newton meters. |
| [`NijMycNCE`](nijmycnce.md) |  |
| [`NijMycNCF`](nijmycncf.md) |  |
| [`NijMycNTF`](nijmycntf.md) |  |
| [`NijNCE`](nijnce.md) | Specifies whether DIAdem executes the Nij calculation after NCE. |
| [`NijNCF`](nijncf.md) | Specifies whether DIAdem executes the Nij calculation after NCF. |
| [`NijNormalizedOutput`](nijnormalizedoutput.md) | Specifies whether DIAdem normalizes the result values ranging from -1 to +1. |
| [`NijNTE`](nijnte.md) | Specifies whether DIAdem executes the Nij calculation after NTE. |
| [`NijNTF`](nijntf.md) | Specifies whether DIAdem executes the Nij calculation after NTF. |
| [`NijTime`](nijtime.md) | Receives the time value for the maximum value. |
| [`NijType`](nijtype.md) | Specifies the calculation type. |
| [`NijVersion`](nijversion.md) | Receives the version number of the Nij calculation routine. |
| [`NoMasterLayout`](nomasterlayout.md) |  |
| [`NonLinearFitClipCopy`](nonlinearfitclipcopy.md) | Specifies whether DIAdem transfers the results of a non-linear curve fit to the clipboard. |
| [`NonLinearFitClipValue`](nonlinearfitclipvalue.md) | Specifies whether DIAdem transfers the results of a non-linear curve fit to the clipboard as a value or as a variable reference. |
| [`NonLinearFitCoef`](nonlinearfitcoef.md) | Receives the coefficients of a non-linear curve fitting setup function. |
| [`NonLinearFitCoefCount`](nonlinearfitcoefcount.md) | Specifies the number of coefficients in the setup function of a non-linear curve fitting. |
| [`NonLinearFitCoefName`](nonlinearfitcoefname.md) | Specifies the names of the coefficients in the setup function of a non-linear curve fitting. |
| [`NonLinearFitCovariance`](nonlinearfitcovariance.md) | Specifies whether DIAdem generates the covariance matrix for a non-linear curve fitting. |
| [`NonLinearFitFctStr`](nonlinearfitfctstr.md) | Receives the setup function used by a non-linear curve fit. |
| [`NonLinearFitIndepVariable`](nonlinearfitindepvariable.md) | Specifies the name of the independent variable in the setup function of a non-linear curve fitting. |
| [`NonLinearFitInitCoef`](nonlinearfitinitcoef.md) | Specifies the initially received values for the coefficients of the setup function of a non-linear curve fitting. The success of the curve fitting depends on how close the initial values are to the result. |
| [`NonLinearFitMaxIterations`](nonlinearfitmaxiterations.md) | Specifies the maximum number of the fitting routine iterations of a non-linear curve fitting. If the number of iterations exceeds this value, the fitting process stops. |
| [`NonLinearFitModelFunction`](nonlinearfitmodelfunction.md) | Specifies the formula string of the setup function for the non-linear curve fitting in VBS syntax. You cannot use the characters e and pi as coefficients because the characters are DIAdem constants for the Eulerian number and the circle number. |
| [`NonLinearFitMSE`](nonlinearfitmse.md) | Receives the mean squared error of a non-linear curve fitting. |
| [`NonLinearFitWeighted`](nonlinearfitweighted.md) | Specifies whether DIAdem weights the y-values in a non-linear curve fitting. |
| [`NoVChnX`](novchnx.md) | Specifies whether DIAdem processes one data channel or several. If the value is TRUE , DIAdem processes only one channel. |
| [`NoVCtrlChn`](novctrlchn.md) | Specifies whether DIAdem searches for NoValues only in the x-channel or also in the y-channels. |
| [`NoVMeth`](novmeth.md) | Specifies whether DIAdem replaces NoValues with linearly-interpolated or specified values, or whether DIAdem deletes NoValues. |
| [`NovReplaceVal`](novreplaceval.md) | Specifies the value with which DIAdem replaces NoValues . The default value of the NovReplaceVal variable is 0 . |
| [`NoVTargetChn`](novtargetchn.md) | Specifies in which channels DIAdem saves the results of the NoValue operation. |
| [`Nv`](nv.md) | Valid names: Nv, Novalue |
| [`O1`](o1.md) | Specifies a freely usable variant variable. |
| [`O10`](o10.md) | Specifies a freely usable variant variable. |
| [`O2`](o2.md) | Specifies a freely usable variant variable. |
| [`O3`](o3.md) | Specifies a freely usable variant variable. |
| [`O4`](o4.md) | Specifies a freely usable variant variable. |
| [`O5`](o5.md) | Specifies a freely usable variant variable. |
| [`O6`](o6.md) | Specifies a freely usable variant variable. |
| [`O7`](o7.md) | Specifies a freely usable variant variable. |
| [`O8`](o8.md) | Specifies a freely usable variant variable. |
| [`O9`](o9.md) | Specifies a freely usable variant variable. |
| [`ObjDelta`](objdelta.md) | Specifies by how many layers DIAdem moves the object. |
| [`ObjectNoMax`](objectnomax.md) | Specifies the maximum possible number of objects in DIAdem REPORT. |
| [`ObjType`](objtype.md) |  |
| [`OffsetCorrection`](offsetcorrection.md) | Determines whether DIAdem subtracts the first time value as offset from the subsequent time values. |
| [`OffsetStartTime`](offsetstarttime.md) | Specifies the start time DIAdem adds as an offset to the numeric values. You create time offsets, for example, with the commands TTR or CreateTime . |
| [`OIVDeltaX`](oivdeltax.md) | Specifies the distance between the theoretical head and the theoretical impact surface in x-direction in meters. |
| [`OIVDeltaY`](oivdeltay.md) | Specifies the distance between the theoretical head and the theoretical impact surface in y-direction in meters. |
| [`OIVDistance`](oivdistance.md) | Specifies the distance between the theoretical head and the vehicle center of gravity in meters. |
| [`OIVTimeFlight`](oivtimeflight.md) | Receives the period of time in seconds during which the impact moves the passengers. |
| [`OIVVelocity`](oivvelocity.md) | Receives the impact velocity of the passengers in kilometers per hour. |
| [`OIVVersion`](oivversion.md) | Receives the version number of the OIV calculation routine. |
| [`OLEChnCol`](olechncol.md) |  |
| [`OLEChnRow`](olechnrow.md) |  |
| [`OLECmdText`](olecmdtext.md) |  |
| [`OLEDisconnect`](oledisconnect.md) |  |
| [`OLEFloatResult`](olefloatresult.md) |  |
| [`OLEIntResult`](oleintresult.md) |  |
| [`OLELockMode`](olelockmode.md) | Specifies the status of the OLE interfaces TOCommand and TODataSheet . |
| [`OLEServerHandle`](oleserverhandle.md) |  |
| [`OLEState`](olestate.md) |  |
| [`OLETextResult`](oletextresult.md) |  |
| [`OnCallingHelp`](oncallinghelp.md) | Specifies which user command DIAdem executes when the Help is called. |
| [`OnF1KeyPressed`](onf1keypressed.md) | Specifies the user command DIAdem executes when you press F1. DIAdem does not execute this function in a user dialog box. Instead use the EventFuncKeyPressed event in user dialog boxes. You cannot assign several user commands to the OnF1KeyPressed event. |
| [`OnFilterDroppedFile`](onfilterdroppedfile.md) | Specifies the user command that DIAdem executes when you drag and drop one or more files onto DIAdem. DIAdem does not execute this function when you drag the files onto DIAdem SCRIPT. You cannot assign several user commands to the OnFilterDroppedFile event. |
| [`OnFilterKeyShortcut`](onfilterkeyshortcut.md) | Specifies the user function DIAdem executes when you press <Shift>, <Ctrl>, or <Alt> button combinations. DIAdem does not execute this function when you execute the shortcut in DIAdem SCRIPT. You cannot assign several user commands to the OnFilterKeyShortcut event. |
| [`OnPanelChanged`](onpanelchanged.md) | Specifies the command that DIAdem executes when DIAdem switches to another DIAdem panel. |
| [`OnPicUpdateEnd`](onpicupdateend.md) |  |
| [`OnPicUpdatePageE`](onpicupdatepagee.md) |  |
| [`OnPicUpdatePageS`](onpicupdatepages.md) |  |
| [`OnPicUpdateStart`](onpicupdatestart.md) |  |
| [`OpenBoundClass`](openboundclass.md) | Specifies whether DIAdem counts values outside the class limits. |
| [`OptimizeDataTypeIP`](optimizedatatypeip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result channels of the data optimization. |
| [`OptimizeDataTypeRoundDigitCount`](optimizedatatyperounddigitcount.md) | Specifies how many places DIAdem rounds in order to optimize the data. |
| [`OptimizeDataTypeRoundDigitType`](optimizedatatyperounddigittype.md) | Specifies which places DIAdem rounds in order to optimize the data. |
| [`OptimizeDataTypeRoundMode`](optimizedatatyperoundmode.md) | Specifies the rounding mode for data optimization. |
| [`ORAMax`](oramax.md) | Receives the stoppage deceleration after the impact in gn (gravity acceleration). |
| [`ORATime`](oratime.md) | Receives the time of the stoppage deceleration. |
| [`ORATime0`](oratime0.md) | Specifies the time of collision in seconds. |
| [`ORAVersion`](oraversion.md) | Receives the version number of the ORA calculation routine. |
| [`OrdAFFFTLength`](ordaffftlength.md) | Specifies the interval length of the FFT for order analysis in the frequency domain. |
| [`OrdAFFiltRecalc`](ordaffiltrecalc.md) | Specifies after how many rotations an order analysis in the frequency domain recalculates the filter coefficients. |
| [`OrdAFMaxOrder`](ordafmaxorder.md) | Specifies  the maximum possible order for an order analysis in the frequency range. |
| [`OrdAFRevolStep`](ordafrevolstep.md) | Specifies the step width of the rpm generation for an order analysis in the frequency range. |
| [`OrdAFSigRefValue`](ordafsigrefvalue.md) | Specifies the reference value when evaluating the results of the order analysis in the frequency area. |
| [`OrdAFSigWeight`](ordafsigweight.md) | Specifies how DIAdem evaluates the results of the order analysis in the frequency domain. |
| [`OrdAFType`](ordaftype.md) | In an order analysis this variable specifies whether DIAdem calculates frequencies or orders in the frequency range. |
| [`OrdATOCalcMode`](ordatocalcmode.md) | Specifies whether DIAdem runs third or octave analyses. |
| [`OrdATOFiltRecalc`](ordatofiltrecalc.md) | In an order analysis this variable specifies after how many rotations DIAdem recalculates the filter coefficients. |
| [`OrdATOFreqMax`](ordatofreqmax.md) | Specifies the upper center frequency of the third/octave analysis. |
| [`OrdATOFreqMin`](ordatofreqmin.md) | Specifies the lower center frequency of the third/octave analysis. |
| [`OrdATOOrdCalc`](ordatoordcalc.md) | Specifies whether DIAdem calculates orders. |
| [`OrdATOOrdLst`](ordatoordlst.md) | Specifies the orders to be calculated. |
| [`OrdATORedBegin`](ordatoredbegin.md) | In an order analysis this variable specifies the start rpm for data reduction in relation to rpm. |
| [`OrdATORedEnd`](ordatoredend.md) | In an order analysis this variable specifies the end rpm for data reduction in relation to rpm. |
| [`OrdATORedFactor`](ordatoredfactor.md) | In an order analysis this variable specifies the reduction factor for data reduction in relation to time. |
| [`OrdATORedStep`](ordatoredstep.md) | In an order analysis this variable specifies the rpm increment for data reduction in relation to rpm. |
| [`OrdATORedType`](ordatoredtype.md) | Specifies whether DIAdem runs the order analysis with the data reduction in relation to time or to rpm. |
| [`OrdATORMS`](ordatorms.md) | Specifies the averaging time for RMS calculations in seconds. |
| [`OrdATOSigRefValue`](ordatosigrefvalue.md) | Specifies the reference value when evaluating the results of the order analysis in the time domain. |
| [`OrdATOSigWeight`](ordatosigweight.md) | Specifies how DIAdem evaluates the results of the order analysis in the time domain. |
| [`OrdATOSum`](ordatosum.md) | Specifies whether DIAdem calculates the sum level of the amplitude channel. The sum level corresponds with the floating square mean over all frequencies of the signal. |
| [`OrderBodeBandwidthBegin`](orderbodebandwidthbegin.md) | Specifies the start value of the bandwidth of an order. |
| [`OrderBodeBandwidthEnd`](orderbodebandwidthend.md) | Specifies the end value of the bandwidth of an order. |
| [`OrderBodeCalcOrder`](orderbodecalcorder.md) | Specifies the orders of the curves to be calculated. |
| [`OrderBodeCPFullChannel`](orderbodecpfullchannel.md) | Specifies whether DIAdem calculates the power spectrum over the entire channel or half the channel during the calculation. |
| [`OrderBodeIntervalLength`](orderbodeintervallength.md) | Specifies the number of values in an interval. |
| [`OrderBodeIntervalType`](orderbodeintervaltype.md) | Specifies the data amount of the calculation. |
| [`OrderBodeNoOfIntervals`](orderbodenoofintervals.md) | Specifies the number of intervals. |
| [`OrderBodeRunoutCompAmplitudeRef`](orderboderunoutcompamplituderef.md) | Specifies the value for the runout correction of the amplitude which DIAdem subtracts from the amplitude calculated for the first order. |
| [`OrderBodeRunoutCompPhaseRef`](orderboderunoutcompphaseref.md) | Specifies the value for the runout correction of the phase which DIAdem subtracts from the phase calculated for the first order. |
| [`OrderBodeWndCorrectType`](orderbodewndcorrecttype.md) | Specifies whether and how DIAdem corrects the damping effect of the window function on the amplitude. |
| [`OrderBodeWndFct`](orderbodewndfct.md) | Specifies the window function. |
| [`OsTmpDrv`](ostmpdrv.md) | Specifies the general temporary path of the operating system. |
| [`OutPutPath`](outputpath.md) | Valid names: OutPutPath, DlgOutputPath |
| [`oValue`](ovalue.md) | Specifies the value of the quantity. |
| [`OverWriteMode`](overwritemode.md) | Specifies whether DIAdem overwrites the values or appends the values. The default value is FALSE , which means that DIAdem appends the values. |
| [`PalNoMax`](palnomax.md) | Specifies the maximum number of entries in the color palette. |
| [`ParaFile`](parafile.md) |  |
| [`ParallelProcessControl`](parallelprocesscontrol.md) | The ParallelProcessControl object provides parallel processing in DIAdem. The ParallelProcessControl object starts more DIAdem applications which run in the background or in the foreground, or you can request the status of a Worker object . |
| [`PartialMode`](partialmode.md) | Specifies whether DIAdem displays the dialog box for channel selection. The default value is FALSE and specifies that DIAdem does not display the dialog box. |
| [`PartToReserve`](parttoreserve.md) | Specifies the percentage of messages at the end of a logfile, which DIAdem does not delete when it resets. |
| [`PathsToBeIndexed`](pathstobeindexed.md) | Specifies a data field that contains the names of the files or paths which the DataFinder is to reindex. You must specify the files with the complete path. If the array contains more than 100 file or path entries, the command creates a further job file. The specified files or folders must be contained in the search areas of the DataFinder server. |
| [`PathsToBeProcessed`](pathstobeprocessed.md) | Specifies an array that contains the names of the files or paths which the DataFinder is to reindex. You must specify the files with the complete path. If the array contains more than 100 file or path entries, the command creates a further job file. The specified files or folders must be contained in the search areas of data preparation. |
| [`PathTitle`](pathtitle.md) | Valid names: PathTitle, DlgPathTitle |
| [`PatternFindAlignPattern`](patternfindalignpattern.md) | Specifies whether DIAdem uses a y-offset. |
| [`PatternFindBandwidth`](patternfindbandwidth.md) | Specifies the maximum number of values by which the signal channel may offset against the pattern channel. |
| [`PatternFindMaxDistance`](patternfindmaxdistance.md) | Specifies the maximum valid deviation of the signal channel to the pattern channel. |
| [`PDFAppend`](pdfappend.md) | Specifies whether DIAdem appends a PDF export to an existing PDF file. The default value is FALSE and specifies that DIAdem does not append the PDF export. |
| [`PdfExportState`](pdfexportstate.md) | Specifies whether the DIAdem PDF printer is installed, and whether a PDF can be exported. |
| [`PDFFileName`](pdffilename.md) | Specifies the name of a PDF file. |
| [`PDFFontsEmbedded`](pdffontsembedded.md) | Specifies whether DIAdem embeds the used fonts in the PDF file. |
| [`PDFFormat`](pdfformat.md) | Specifies whether DIAdem saves the PDF files in the standard format or in the PDF/A archiving format. |
| [`PDFJPGCompressed`](pdfjpgcompressed.md) | Specifies whether DIAdem compresses embedded JPC graphics. |
| [`PDFOptimization`](pdfoptimization.md) | Specifies whether DIAdem optimizes PDF files for fast web display. To do so, DIAdem restructures a PDF document in such a way that it can be downloaded page-wise from a web server. DIAdem does not optimize PDF files by default. If the value is TRUE , DIAdem optimizes PDF files. |
| [`PDFResolution`](pdfresolution.md) | Specifies in PDF files the resolution of graphics. |
| [`PDFUseMicrosoftPrinter`](pdfusemicrosoftprinter.md) | Specifies whether DIAdem uses the Microsoft standard PDF printer available from Windows version 10 onwards. |
| [`PeakDetectThreshold`](peakdetectthreshold.md) | Specifies the threshold up to which DIAdem ignores peaks and valleys. The adapted amplitude of the peaks must not be below the threshold. The adapted amplitude of the valleys must not be above the threshold value. |
| [`PeakDetectType`](peakdetecttype.md) | Specifies the peak types. |
| [`PeakDetectWidth`](peakdetectwidth.md) | Specifies the number of successive points, which DIAdem uses for the adaptation with the least squares method. The value must be greater than or equal to three. The value should be at least half the width of the peaks or valleys and below that if the signals are noiseless. If the widths are large, you can decrease the apparent peak amplitudes and move the apparent position. If the data is noisy, this change is insignificant because the noise hides the actual peak. Select the smallest possible width, which is still large enough to preclude incorrect peak values created by noise. |
| [`PeakNo`](peakno.md) | Specifies the maximum number of minimum or maximum values DIAdem searches for. |
| [`PeakNoMax`](peaknomax.md) | Specifies the maximum number of peaks you can search for during a peak search. |
| [`PeakSort`](peaksort.md) | Specifies the order in which DIAdem searches for minimum values or maximum values. |
| [`PeakType`](peaktype.md) | Specifies whether DIAdem searches for minimum values or maximum values. |
| [`PhaseUnwrapBegin`](phaseunwrapbegin.md) | Specifies the smallest value of the input channel. |
| [`PhaseUnwrapEnd`](phaseunwrapend.md) | Specifies the greatest value of the input channel. |
| [`PhaseWrapBegin`](phasewrapbegin.md) | Specifies the smallest value of the input channel. |
| [`PhaseWrapEnd`](phasewrapend.md) | Specifies the greatest value of the input channel. |
| [`PHDMax`](phdmax.md) | Receives the maximum head deceleration after the impact in gn (acceleration of gravity). |
| [`PHDTime`](phdtime.md) | Receives the time for the maximum head delay, in seconds. |
| [`PHDTime0`](phdtime0.md) | Specifies the time of collision of the theoretical head with the theoretical impact surface, in seconds. |
| [`PHDVersion`](phdversion.md) | Receives the version number of the PHD calculation routine. |
| [`PicBackColor`](picbackcolor.md) |  |
| [`PicBackColorRGB`](picbackcolorrgb.md) |  |
| [`PicBackColorRGB2`](picbackcolorrgb2.md) |  |
| [`PicBackFMode`](picbackfmode.md) |  |
| [`PicBackFVariant`](picbackfvariant.md) |  |
| [`PicComment`](piccomment.md) |  |
| [`PicCutOutXBegin`](piccutoutxbegin.md) |  |
| [`PicCutOutXChnTyp`](piccutoutxchntyp.md) |  |
| [`PicCutOutXEnd`](piccutoutxend.md) |  |
| [`PicCutOutXKey`](piccutoutxkey.md) |  |
| [`PicDefByIdent`](picdefbyident.md) |  |
| [`PicDefExpand`](picdefexpand.md) |  |
| [`PicDefExpandMode`](picdefexpandmode.md) |  |
| [`PicDefExpLColor`](picdefexplcolor.md) |  |
| [`PicDefExpLColRGB`](picdefexplcolrgb.md) |  |
| [`PicDefExpLColUse`](picdefexplcoluse.md) |  |
| [`PicDefExpLInterv`](picdefexplinterv.md) |  |
| [`PicDefExpLIntUse`](picdefexplintuse.md) |  |
| [`PicDefExpListUse`](picdefexplistuse.md) |  |
| [`PicDefExpLType`](picdefexpltype.md) |  |
| [`PicDefExpLTypUse`](picdefexpltypuse.md) |  |
| [`PicDefExpLWidth`](picdefexplwidth.md) |  |
| [`PicDefExpLWidUse`](picdefexplwiduse.md) |  |
| [`PicDefExpMark`](picdefexpmark.md) |  |
| [`PicDefExpMarkBType`](picdefexpmarkbtype.md) |  |
| [`PicDefExpMarkColor`](picdefexpmarkcolor.md) |  |
| [`PicDefExpMarkColorAuto`](picdefexpmarkcolorauto.md) |  |
| [`PicDefExpMarkColorRGB`](picdefexpmarkcolorrgb.md) |  |
| [`PicDefExpMarkEType`](picdefexpmarketype.md) |  |
| [`PicDefExpMarkFillColor`](picdefexpmarkfillcolor.md) |  |
| [`PicDefExpMarkFillColorAuto`](picdefexpmarkfillcolorauto.md) |  |
| [`PicDefExpMarkFillColorRGB`](picdefexpmarkfillcolorrgb.md) |  |
| [`PicDefExpMarkLWidth`](picdefexpmarklwidth.md) |  |
| [`PicDefExpMarkNType`](picdefexpmarkntype.md) |  |
| [`PicDefExpMarkParamUse`](picdefexpmarkparamuse.md) |  |
| [`PicDefExpMarkRMode`](picdefexpmarkrmode.md) |  |
| [`PicDefExpMarkRType`](picdefexpmarkrtype.md) |  |
| [`PicDefExpMarkSize`](picdefexpmarksize.md) |  |
| [`PicDefExpMarkUse`](picdefexpmarkuse.md) |  |
| [`PicDefExpNo`](picdefexpno.md) |  |
| [`PicDescription`](picdescription.md) |  |
| [`PicDoubleBuffer`](picdoublebuffer.md) |  |
| [`PicFile`](picfile.md) |  |
| [`PicFileCode`](picfilecode.md) |  |
| [`PicFileExt`](picfileext.md) |  |
| [`PicFrame`](picframe.md) |  |
| [`PicFrameColor`](picframecolor.md) |  |
| [`PicFrameColorRGB`](picframecolorrgb.md) |  |
| [`PicFrameLWidth`](picframelwidth.md) |  |
| [`PicGlobClip`](picglobclip.md) |  |
| [`PicHeightInScal`](picheightinscal.md) |  |
| [`PicInScal`](picinscal.md) |  |
| [`PicIsChanged`](picischanged.md) |  |
| [`PicObjHighlight`](picobjhighlight.md) | Specifies whether DIAdem highlights objects in a REPORT layout when you move the mouse across an object you want to select. |
| [`PicObjMaxSize`](picobjmaxsize.md) |  |
| [`PicObjMinSize`](picobjminsize.md) |  |
| [`PicObjType`](picobjtype.md) |  |
| [`PicPageHeight`](picpageheight.md) |  |
| [`PicPageOrient`](picpageorient.md) |  |
| [`PicPageRatio`](picpageratio.md) |  |
| [`PicPageWidth`](picpagewidth.md) |  |
| [`PicPalColNo`](picpalcolno.md) |  |
| [`PicPalCtrlHSL`](picpalctrlhsl.md) |  |
| [`PicPalLineInterv`](picpallineinterv.md) |  |
| [`PicPalLineType`](picpallinetype.md) |  |
| [`PicPalLineWidth`](picpallinewidth.md) |  |
| [`PicPalValBegin`](picpalvalbegin.md) |  |
| [`PicPalValEnd`](picpalvalend.md) |  |
| [`PicPalValType`](picpalvaltype.md) |  |
| [`PicRatio`](picratio.md) |  |
| [`PicScaleNorm`](picscalenorm.md) |  |
| [`PicUpdateOnObjChange`](picupdateonobjchange.md) | Specifies whether DIAdem replots the entire worksheet after you have changed individual objects. DIAdem saves this information in the desktop file. |
| [`PicUseLocalParam`](picuselocalparam.md) |  |
| [`PicWidthInScal`](picwidthinscal.md) |  |
| [`PolynomialOrder`](polynomialorder.md) | Specifies the order of the polynomial. |
| [`Portal`](portal.md) | Specifies the Portal object that provides access to the subobjects, methods, and properties in the Data Portal. |
| [`PrgBetaRevision`](prgbetarevision.md) | Specifies the Beta revision number of DIAdem. |
| [`PrintColor`](printcolor.md) | Specifies whether DIAdem prints in color, in black and white, or in the color setting configured on the printer. |
| [`PrintCopies`](printcopies.md) | Specifies the number of print copies. |
| [`PrintDevice`](printdevice.md) | Specifies the printer. |
| [`PrinterAvailable`](printeravailable.md) | Specifies whether a printer is available in your system. |
| [`PrinterName`](printername.md) | Valid names: PrinterName, PrintName |
| [`PrinterState`](printerstate.md) | Specifies the status of the standard Windows printer. |
| [`PrintFile`](printfile.md) |  |
| [`PrintFromPage`](printfrompage.md) | Specifies the first page that DIAdem prints if you only print certain pages of a report. |
| [`PrintHeight`](printheight.md) | Valid names: PrintHeight, PrintHeigth |
| [`PrintLeftMarg`](printleftmarg.md) | Specifies the distance of the printout from the left edge of the sheet. |
| [`PrintOrient`](printorient.md) | Specifies the page alignment for printed graphics. |
| [`PrintRangeType`](printrangetype.md) | Specifies whether DIAdem prints all pages of a report or only certain pages of a report. |
| [`PrintToPage`](printtopage.md) | Specifies the last page that DIAdem prints if you only print certain pages of a report. |
| [`PrintTopMarg`](printtopmarg.md) | Specifies the distance of the printout to the top edge of the sheet. |
| [`PrintWidth`](printwidth.md) | Specifies the width of the printout. |
| [`ProgramBuild`](programbuild.md) | Receives the DIAdem build number. |
| [`ProgramDrv`](programdrv.md) | Specifies the path and the folder where DIAdem is installed. |
| [`ProgramErrorNo`](programerrorno.md) | Specifies the current DIAdem error number. |
| [`ProgramRevision`](programrevision.md) | Receives the DIAdem version number multiplied by 100. |
| [`ProgramVersion`](programversion.md) | Receives the DIAdem version number. |
| [`ProgramVersionName`](programversionname.md) | Specifies the name of a DIAdem version. |
| [`PropInheritanceMode`](propinheritancemode.md) | Specifies whether DIAdem transfers properties of elements from superordinate levels when loading an element from a ASAM data store to the element in the Data Portal. DIAdem only uses the settings you make here if you select Same as NAVIGATOR Settings in the Edit Loading Configuration dialog box. |
| [`PropInheritanceModeDF`](propinheritancemodedf.md) | Specifies whether DIAdem transfers properties of elements from superordinate levels when loading a file or an element from a DataFinder to the element in the Data Portal. |
| [`PropInheritanceSeparator`](propinheritanceseparator.md) | Specifies whether DIAdem uses the underscore or the tilde as the separator for the inheritance of properties. |
| [`PropIsFixed`](propisfixed.md) |  |
| [`PropIsReadOnly`](propisreadonly.md) |  |
| [`PropIsVisible`](propisvisible.md) |  |
| [`PropName`](propname.md) |  |
| [`PropNamingSchema`](propnamingschema.md) | Specifies the name pattern of properties after the properties are loaded into the Data Portal. If you load data from an ASAM data store into the Data Portal, DIAdem names the properties in the Data Portal according to these rules. DIAdem only uses the settings you make here if you select Same as NAVIGATOR Settings in the Edit Loading Configuration dialog box. |
| [`PropTextValue`](proptextvalue.md) |  |
| [`PropValue`](propvalue.md) |  |
| [`PtlFloating`](ptlfloating.md) | Specifies whether DIAdem displays the Data Portal in floating mode. |
| [`PtlInFullScreen`](ptlinfullscreen.md) | Specifies whether DIAdem hides the Data Portal in full-screen mode. |
| [`PtlShow`](ptlshow.md) | Specifies whether the Data Portal is enabled or disabled. |
| [`PtlVisible`](ptlvisible.md) | Specifies whether the Data Portal is visible. |
| [`PulseDetHysteresisType`](pulsedethysteresistype.md) | Specifies whether DIAdem interprets the hysteresis as an absolute numeric value or as a percentage. If you select Percentage , the hysteresis refers to the range between the global minimum and maximum of the current tachometer channel. |
| [`PulseDetHysteresisValue`](pulsedethysteresisvalue.md) | Specifies the minimum range in addition to the threshold, which the pulse must have. This is to prevent disturbances. |
| [`PulseDetInterpolMissValues`](pulsedetinterpolmissvalues.md) | Specifies whether DIAdem uses linear interpolation to add missing pulses. |
| [`PulseDetPulseRevolution`](pulsedetpulserevolution.md) | Specifies the number of pulses for one revolution. |
| [`PulseDetPulseWidth`](pulsedetpulsewidth.md) | Specifies the minimum width of a pulse. The default value is 2 , which means that two consecutive tachometer values must reach the threshold for a pulse to be detected. |
| [`PulseDetResultType`](pulsedetresulttype.md) | Specifies the results of the tachometer signal evaluation. |
| [`PulseDetSlope`](pulsedetslope.md) | Specifies whether the pulse must increase or decrease. |
| [`PulseDetThresholdType`](pulsedetthresholdtype.md) | Specifies whether DIAdem interprets the threshold value as an absolute numeric value or as a percentage. If you select Percentage , the threshold refers to the range between the global minimum and maximum of the current tachometer channel. |
| [`PulseDetThresholdValue`](pulsedetthresholdvalue.md) | Specifies the threshold which the signal must exceed in order to be validated as a pulse. |
| [`PulseLimit`](pulselimit.md) | Specifies whether the measured acceleration values are all within the specified range. |
| [`PulseLimitTIdx`](pulselimittidx.md) | Receives the number of the first point outside the given range. |
| [`PulseLimitVer`](pulselimitver.md) | Valid names: PulseLimitVer, PulseLimitVersion |
| [`QuantRangeMax`](quantrangemax.md) | Specifies the top range limit up to which DIAdem divides a channel. |
| [`QuantRangeMin`](quantrangemin.md) | Specifies the bottom range limit where DIAdem starts dividing a channel. |
| [`QuantResolution`](quantresolution.md) | Specifies the number of steps into which DIAdem divides a channel. |
| [`QueryDrv`](querydrv.md) |  |
| [`R1`](r1.md) | Specifies a freely usable real variable. |
| [`R10`](r10.md) | Specifies a freely usable real variable. |
| [`R11`](r11.md) | Specifies a freely usable real variable. |
| [`R12`](r12.md) | Specifies a freely usable real variable. |
| [`R13`](r13.md) | Specifies a freely usable real variable. |
| [`R14`](r14.md) | Specifies a freely usable real variable. |
| [`R15`](r15.md) | Specifies a freely usable real variable. |
| [`R16`](r16.md) | Specifies a freely usable real variable. |
| [`R17`](r17.md) | Specifies a freely usable real variable. |
| [`R18`](r18.md) | Specifies a freely usable real variable. |
| [`R19`](r19.md) | Specifies a freely usable real variable. |
| [`R2`](r2.md) | Specifies a freely usable real variable. |
| [`R20`](r20.md) | Specifies a freely usable real variable. |
| [`R21`](r21.md) | Specifies a freely usable real variable. |
| [`R22`](r22.md) | Specifies a freely usable real variable. |
| [`R23`](r23.md) | Specifies a freely usable real variable. |
| [`R24`](r24.md) | Specifies a freely usable real variable. |
| [`R25`](r25.md) | Specifies a freely usable real variable. |
| [`R26`](r26.md) | Specifies a freely usable real variable. |
| [`R27`](r27.md) | Specifies a freely usable real variable. |
| [`R28`](r28.md) | Specifies a freely usable real variable. |
| [`R29`](r29.md) | Specifies a freely usable real variable. |
| [`R3`](r3.md) | Specifies a freely usable real variable. |
| [`R30`](r30.md) | Specifies a freely usable real variable. |
| [`R31`](r31.md) | Specifies a freely usable real variable. |
| [`R32`](r32.md) | Specifies a freely usable real variable. |
| [`R4`](r4.md) | Specifies a freely usable real variable. |
| [`R5`](r5.md) | Specifies a freely usable real variable. |
| [`R6`](r6.md) | Specifies a freely usable real variable. |
| [`R7`](r7.md) | Specifies a freely usable real variable. |
| [`R8`](r8.md) | Specifies a freely usable real variable. |
| [`R9`](r9.md) | Specifies a freely usable real variable. |
| [`RainChnContain`](rainchncontain.md) | Specifies whether DIAdem stores the class numbers or the values of the class means. |
| [`RainInclFirstLastVal`](raininclfirstlastval.md) | Specifies whether DIAdem uses the first and the last value of the signal that is to be classified as the reversal points in a rainflow classification. |
| [`RainMatExist`](rainmatexist.md) | Specifies whether DIAdem uses a transition matrix or a rainflow matrix. |
| [`RainMatTrans`](rainmattrans.md) | Specifies whether DIAdem stores the results of the rainflow matrix and the transition matrix in the Data Portal. |
| [`RainOneParaCalc`](rainoneparacalc.md) | Specifies whether DIAdem stores the range counting from the transition matrix for rising ranges. |
| [`RainResiduumCalc`](rainresiduumcalc.md) | Specifies whether DIAdem includes the residues in the count. |
| [`RainSpecOnePara`](rainspeconepara.md) | Specifies whether DIAdem stores the range counting from the transition matrix for falling ranges. |
| [`RdeEuFuelAlpha`](rdeeufuelalpha.md) | Specifies the molar ratio of hydrogen (H/C) in the fuel. |
| [`RdeEuFuelBeta`](rdeeufuelbeta.md) | Specifies the molar ratio of carbon (C/C) in the fuel. |
| [`RdeEuFuelDelta`](rdeeufueldelta.md) | Specifies the molar ratio of nitrogen (N/C) in the fuel. |
| [`RdeEuFuelEpsilon`](rdeeufuelepsilon.md) | Specifies the molar ratio of oxygen (O/C) in the fuel. |
| [`RdeEuFuelExhaustGasDensity`](rdeeufuelexhaustgasdensity.md) | Specifies the exhaust gas density in kilograms per cubic meter. |
| [`RdeEuFuelGamma`](rdeeufuelgamma.md) | Specifies the molar ratio of sulfur (S/C) in the fuel. |
| [`RdeEuFuelK_CH4`](rdeeufuelk-ch4.md) | Specifies the density ratio of methane to the total density of the exhaust gas. |
| [`RdeEuFuelK_CO`](rdeeufuelk-co.md) | Specifies the density ratio of carbon monoxide to the total density of the exhaust gas. |
| [`RdeEuFuelK_CO2`](rdeeufuelk-co2.md) | Specifies the density ratio of carbon dioxide to the total density of the exhaust gas. |
| [`RdeEuFuelK_NOx`](rdeeufuelk-nox.md) | Specifies the density ratio of nitrogen to the total density of the exhaust gas. |
| [`RdeEuFuelK_THC`](rdeeufuelk-thc.md) | Specifies the density ratio of hydrocarbons to the total density of the exhaust gas. |
| [`RdeEuFuelName`](rdeeufuelname.md) | Specifies the name of the fuel that is used. |
| [`RdeEuFuelType`](rdeeufueltype.md) | Specifies the fuel to use. |
| [`RdeEuMaxNoOfFuelTypes`](rdeeumaxnooffueltypes.md) | Specifies the maximum number of fuel types used. |
| [`RdeEuMinNoOfFuelTypes`](rdeeuminnooffueltypes.md) | Specifies the minimum number of fuel types used. |
| [`RdeEuNoOfFuelTypes`](rdeeunooffueltypes.md) | Specifies the number of fuel types used. |
| [`RdeEuPropulsionType`](rdeeupropulsiontype.md) | Specifies the propulsion type. |
| [`RdeEuVehicleCategory`](rdeeuvehiclecategory.md) | Specifies the vehicle category according to Annex II of Directive 70/156/EEC, such as M , M1 . |
| [`RdeEuWLTPCO2ReferenceMass`](rdeeuwltpco2referencemass.md) | Determines the reference value for the mass of carbon dioxide in kilograms. |
| [`RdeEuWLTPExtraHighSpeed`](rdeeuwltpextrahighspeed.md) | Defines the reference point for the phase of the WLTP cycle at very high speed. |
| [`RdeEuWLTPHighSpeed`](rdeeuwltphighspeed.md) | Specifies the reference point for the high-speed phase of the WLTP cycle. |
| [`RdeEuWLTPLowSpeed`](rdeeuwltplowspeed.md) | Defines the reference point for the phase of the WLTP cycle at very low speed. |
| [`RecMode`](recmode.md) | Valid names: RecMode, WriteMode |
| [`RedBegin`](redbegin.md) | Specifies the first data channel value that is to be included. |
| [`RedChannel`](redchannel.md) | Valid names: RedChannel, RedChannelNo |
| [`RedEnd`](redend.md) | Specifies the last data channel value that is to be included. |
| [`RedInterv`](redinterv.md) | Specifies the number of values in an interval. |
| [`RedMethod`](redmethod.md) | Specifies the parameters for defining an interval. |
| [`RedNo`](redno.md) | Specifies the number of intervals that DIAdem reduces. |
| [`RedType`](redtype.md) | Specifies the data reduction method. |
| [`ReductionType`](reductiontype.md) | Specifies the data reduction method. You can select several reduction methods simultaneously. DIAdem creates a new data channel for each reduction method. |
| [`RedXChannelNo`](redxchannelno.md) | Specifies the x-channel of the data reduction. |
| [`RegClipCopy`](regclipcopy.md) | Specifies whether DIAdem transfers the results of a regression to the clipboard. |
| [`RegClipValue`](regclipvalue.md) | Specifies whether DIAdem transfers the results of a regression to the clipboard as values or as variable references. |
| [`RegFctStr`](regfctstr.md) | Specifies the format that DIAdem uses to copy regression results to the clipboard. |
| [`RegrCoeffA`](regrcoeffa.md) | Receives the regression coefficient a. |
| [`RegrCoeffB`](regrcoeffb.md) | Receives the regression coefficient b. |
| [`RegrName`](regrname.md) | Receives the name of the regression type to use. |
| [`RegrPrecision`](regrprecision.md) | Receives the coefficient of determination of a regression. |
| [`RegrType`](regrtype.md) | Specifies the setup function for a regression. |
| [`ReplaceWithNoValue`](replacewithnovalue.md) | Specifies that DIAdem replaces the values in the numeric channel with NoValues, which are connected to assignments in the assignment channel. The default value of the variable is FALSE , so that DIAdem does not replace the values originally connected with assignments with NoValues. |
| [`Report`](report.md) | Specifies the Report object that provides access to the objects in DIAdem REPORT. |
| [`ReportAutomaticPrintSizing`](reportautomaticprintsizing.md) | Specifies the minimum margins for the selected printer and the specified page format. |
| [`ReportCurveCoordinateEnableInLegend`](reportcurvecoordinateenableinlegend.md) | Specifies whether DIAdem displays this coordinate in the legend when creating coordinates interactively. |
| [`ReportCurveCoordinateSubsequentToCurve`](reportcurvecoordinatesubsequenttocurve.md) | Specifies whether DIAdem sorts the coordinate into the curve list directly behind the selected curve, when creating coordinates interactively. |
| [`ReportCustomPPTTemplate`](reportcustomppttemplate.md) | Specifies the PowerPoint template which DIAdem uses for PowerPoint export if the variable ReportUseCustomPPTTemplate has the value TRUE . |
| [`ReportDefFont`](reportdeffont.md) | Specifies the character set for all texts and numbers in a report if no character set is specified. |
| [`ReportDefFontTyp`](reportdeffonttyp.md) | Specifies the character set for texts and numbers in a report if no character set is specified. |
| [`ReportDragDropMode`](reportdragdropmode.md) | Specifies the drag and drop behavior in DIAdem REPORT. |
| [`ReportMasterLDrv`](reportmasterldrv.md) | Contains the last selected path to the master layout. |
| [`ReportObj`](reportobj.md) | Valid names: ReportObj, PicObj |
| [`ReportObjLast`](reportobjlast.md) |  |
| [`ReportObjType`](reportobjtype.md) |  |
| [`ReportPrintAsGraphic`](reportprintasgraphic.md) | Specifies whether DIAdem saves the report temporarily as a graphic before DIAdem prints this graphic or displays it as a PDF file. Select this setting if your printer does not correctly display enhanced display options, such as transparent areas. If you select this setting, you cannot select any texts in the PDF documents you have created. |
| [`ReportPrintExpandedPages`](reportprintexpandedpages.md) | Specifies whether DIAdem REPORT prints all pages for automatically expanding tables. You create automatically expanding tables by selecting the entry Automatically increasing for the setting Table length in the Table definition: Scaling dialog box. |
| [`ReportPrintTransparency`](reportprinttransparency.md) | Specifies whether DIAdem includes the transparency of the color when printing. Some printers cannot output transparency and instead print these areas without color. If you disable this setting, DIAdem prints transparent colors opaque without transparency. |
| [`ReportRenderingMode`](reportrenderingmode.md) | Specifies the graphic display quality in DIAdem REPORT. A higher output quality may reduce the display speed. |
| [`ReportReversePrintOrder`](reportreverseprintorder.md) | Specifies that DIAdem REPORT prints the pages in reverse order. |
| [`ReportTemplate`](reporttemplate.md) | Specifies the template for a new worksheet in DIAdem REPORT. |
| [`ReportUnitDisplayMode`](reportunitdisplaymode.md) | Specifies the display mode for the unit for axis labels in DIAdem REPORT if the unit is defined as a DIAdem expression in the label text with square brackets. A DIAdem expression , such as [@@ChnDim(CurrChnNo)@@] , is replaced by the representation of the set mode. |
| [`ReportUseCustomPPTTemplate`](reportusecustomppttemplate.md) | Specifies whether DIAdem uses the PowerPoint template specified in the ReportCustomPPTTemplate variable when exporting from PowerPoint. The default value of the variable is FALSE , so that DIAdem uses the standard PowerPoint template. |
| [`ReportVirtualPrintMemory`](reportvirtualprintmemory.md) | Specifies whether DIAdem manages the temporary printer data in the memory or whether DIAdem outsources the data to the hard drive, when printing and exporting a REPORT layout. DIAdem saves this information in the desktop file. |
| [`ResampleAntiAliasingFilter`](resampleantialiasingfilter.md) | Specifies that DIAdem filters the y input channel. The default value of the variable is FALSE , so that DIAdem does not filter the input channel. |
| [`ResampleCorrelationMode`](resamplecorrelationmode.md) | Specifies whether DIAdem runs the cross correlation calculation in the frequency domain or the time domain. The default value of the variable is “FrequencyDomain” , so that DIAdem executes the calculation in the frequency domain. |
| [`ResampleInterpolateNovalues`](resampleinterpolatenovalues.md) | Specifies that DIAdem replaces the NoValues in the y-values by interpolating the neighboring points. The default value of the variable is FALSE so that DIAdem does not replace NoValues. |
| [`ResampleInterpolationMethod`](resampleinterpolationmethod.md) | Specifies how DIAdem interpolates the y-channels if the ResampleMappingMode variable has the value "Analog" . As a default, the ResampleInterpolationMethod variable has the value "Akima" , which means that DIAdem interpolates the signal with Akima subsplines if you do not specify the value. |
| [`ResampleMappingMode`](resamplemappingmode.md) | Specifies the mapping mode for the resampling. |
| [`ResourceDrv`](resourcedrv.md) | Specifies the path where DIAdem saves internal dialog boxes. |
| [`ResultAngle`](resultangle.md) | Receives the angle in degrees. |
| [`ResultDistance`](resultdistance.md) | Receives the distance in m. |
| [`RMSWidth`](rmswidth.md) | Specifies how many neighboring values are included, as a percentage of the channel length. If there are less values at the boundaries, the calculation runs with less values at one end. |
| [`RootCreateName`](rootcreatename.md) |  |
| [`RootPropCount`](rootpropcount.md) |  |
| [`RootPropName`](rootpropname.md) |  |
| [`RoundDigitCount`](rounddigitcount.md) | Specifies how many places DIAdem rounds. |
| [`RoundDigitType`](rounddigittype.md) | Specifies which places DIAdem rounds. |
| [`RoundIP`](roundip.md) | Specifies whether DIAdem overwrites the values of the input channels with the result channels when rounding. |
| [`RoundMode`](roundmode.md) | Specifies the rounding mode. |
| [`RowLoadAll`](rowloadall.md) | When you add channels from a DAT file, this variable specifies whether you load only certain channels into the Data Portal. |
| [`RowNoStr`](rownostr.md) | Valid names: RowNoStr, BlNo |
| [`RV1`](rv1.md) | Specifies a freely usable real vector. |
| [`RV2`](rv2.md) | Specifies a freely usable real vector. |
| [`RV3`](rv3.md) | Specifies a freely usable real vector. |
| [`SampleFrequency`](samplefrequency.md) | Specifies the sampling rate of the result channel in Hertz. |
| [`SamplingPointChn`](samplingpointchn.md) | Specifies the data channel containing the interpolation points. |
| [`SavitzkyGolayFilterWeighted`](savitzkygolayfilterweighted.md) | Specifies whether DIAdem uses weighting factors when smoothing with the Savitzky-Golay filter. |
| [`ScriptCMDInterfaceName`](scriptcmdinterfacename.md) | Specifies the name of the interface for which DIAdem displays CodeCompletion. |
| [`ScriptCMDItemName`](scriptcmditemname.md) | Specifies the name of the function or variable that was registered as user command or with the GlobDim command. |
| [`ScriptCMDTypeLibName`](scriptcmdtypelibname.md) | Specifies the filename of a TLB file. You can enter the file with the absolute path or a filename. If you do not specify a path, DIAdem expects the file to be in the program directory. |
| [`ScriptExternalPythonIDE`](scriptexternalpythonide.md) | Defines the external development environment (Integrated Development Environment: IDE) for Python files. If you specify a path, you can load Python files from DIAdem SCRIPT into the specified IDE. |
| [`ScriptFile`](scriptfile.md) | Specifies the name of a script file. |
| [`ScriptLibrPath`](scriptlibrpath.md) | Specifies the current SCRIPT library path for scripts. |
| [`ScriptReadPath`](scriptreadpath.md) | Specifies the current read path for scripts. |
| [`ScriptScope`](scriptscope.md) | Specifies the name space of a script. By default the ScriptCode variable contains an empty text. |
| [`ScriptWritePath`](scriptwritepath.md) | Specifies the current write path for scripts. |
| [`SectionBegin`](sectionbegin.md) | Specifies the first channel line index of the channel section that DIAdem loads. |
| [`SectionEnd`](sectionend.md) | Specifies the last channel line index of the channel section that DIAdem loads. |
| [`SeismicLTAWidth`](seismicltawidth.md) | Specifies the time span for calculating the long-term average (LTA) in seconds. The LTA corresponds with the background noise of a seismic signal. |
| [`SeismicPArrivals`](seismicparrivals.md) | Receives the index and arrival time of the P waves of a seismic event in a two-dimensional array. |
| [`SeismicPPhaseDuration`](seismicpphaseduration.md) | Specifies the minimum peak duration in seconds for DIAdem to recognize the peaks as P waves of a seismic event. |
| [`SeismicSArrivals`](seismicsarrivals.md) | Receives the index and arrival time of the S waves of a seismic event in a two-dimensional array. |
| [`SeismicSignalNoiseRatio`](seismicsignalnoiseratio.md) | Specifies the ratio of short-term average to long-term average. The ratio of the two mean values must exceed a threshold for DIAdem to detect the P waves of a seismic event. |
| [`SeismicSPhasePickMode`](seismicsphasepickmode.md) | Specifies whether DIAdem uses the largest peak or the first peak to determine the S phase of a seismic event. |
| [`SeismicSTAWidth`](seismicstawidth.md) | Specifies the time span for calculating the short-term average (STA) in seconds. When calculating the STA mean value, outliers like a single impact have only a minor effect, while persistently high amplitudes of a P wave result in a high mean value. |
| [`SelAllObjCount`](selallobjcount.md) |  |
| [`SelectedChannels`](selectedchannels.md) | Specifies the data channels that DIAdem saves in the target file. If you do not specify any channels, DIAdem saves all channels. |
| [`SelectedObjects`](selectedobjects.md) | Specifies the numbers of the data channels. |
| [`SelMainObjCount`](selmainobjcount.md) |  |
| [`SelObjName`](selobjname.md) |  |
| [`SelObjSubCount`](selobjsubcount.md) |  |
| [`SelObjType`](selobjtype.md) |  |
| [`ServicePack`](servicepack.md) | Specifies the DIAdem Service Pack that is installed. |
| [`ShaftCenterlineGapRefX`](shaftcenterlinegaprefx.md) | Specifies the x-margin to the shaft centerline. |
| [`ShaftCenterlineGapRefY`](shaftcenterlinegaprefy.md) | Specifies the y-margin to the shaft centerline. |
| [`ShaftCenterlineIntervalLength`](shaftcenterlineintervallength.md) | Specifies the number of values in an interval. |
| [`ShaftCenterlineIntervalType`](shaftcenterlineintervaltype.md) | Specifies the data amount for the calculation. |
| [`ShaftCenterlineNoOfIntervals`](shaftcenterlinenoofintervals.md) | Specifies the number of intervals. |
| [`SharedDataPath`](shareddatapath.md) | Specifies a cross-version data path. |
| [`ShellWizardStart`](shellwizardstart.md) | Specifies whether DIAdem enables the Report Wizard when DIAdem starts. |
| [`SHGetFolderCSIDL`](shgetfoldercsidl.md) | Specifies the folders that DIAdem determines with the SHGetFolderPath function. |
| [`SIcum`](sicum.md) | Receives the result of the SI calculation. |
| [`SINADDetectedFrequency`](sinaddetectedfrequency.md) | Receives the fundamental frequency of the signal. |
| [`SINADResult`](sinadresult.md) | Receives the SINAD value (signal to noise and distortion). The SINAD value specifies the signal to distortion ratio in dB. The ratio is defined as the ratio of the effective energy of the input signal to the effective energy of input signals less the energy of the fundamental frequency. |
| [`SINADSearchFrequency`](sinadsearchfrequency.md) | Specifies the approximate center frequency which DIAdem uses to search for the fundamental frequency in the frequency domain. If the value is -1 , DIAdem uses the frequency with the greatest amplitude as fundamental frequency. |
| [`SINADSearchWidth`](sinadsearchwidth.md) | Specifies the relative frequency width to search for the fundamental frequency in the frequency domain. Specify the frequency width as a percentage of the sampling rate. |
| [`SINADTHDPlusNoise`](sinadthdplusnoise.md) | Receives the distortion plus noise. The SINAD value in decibel multiplied by -1 calculates the distortion. |
| [`SingleToneAmplitude`](singletoneamplitude.md) | Receives the amplitude of the single frequency with the greatest amplitude in the input signal. |
| [`SingleToneFrequency`](singletonefrequency.md) | Receives the single frequency with the greatest amplitude in the input signal. |
| [`SingleTonePhase`](singletonephase.md) | Receives the phase of the single frequency with the greatest amplitude in the input signal. |
| [`SingleToneSearchFrequency`](singletonesearchfrequency.md) | Specifies the approximate center frequency which DIAdem uses to search for the fundamental frequency in the frequency domain. If the value is -1 , DIAdem uses the frequency with the greatest amplitude as fundamental frequency. |
| [`SingleToneSearchWidth`](singletonesearchwidth.md) | Specifies the relative frequency width to search for the fundamental frequency in the frequency domain. Specify the frequency width as a percentage of the sampling rate. |
| [`SmoothMode`](smoothmode.md) | Specifies how DIAdem smooths the data channel. The default value is byMeanValue , which means that DIAdem uses the arithmetic mean. |
| [`SmoothType`](smoothtype.md) | Specifies which neighbor values of the value to be smoothed DIAdem uses for the smoothing process. |
| [`SmoothWidth`](smoothwidth.md) | Specifies the number of neighboring values to the left and right of the channel value that DIAdem uses to calculate the mean. |
| [`SortSwitch`](sortswitch.md) | Specifies whether DIAdem only sorts the first data channel. |
| [`SoundActive`](soundactive.md) | Specifies whether DIAdem outputs acoustic signals with messages. |
| [`SoundLevelReferenceValue`](soundlevelreferencevalue.md) | Specifies the reference value for the dB calculation of a sound level. |
| [`SoundLevelResultInDb`](soundlevelresultindb.md) | Determines, whether the result of the ABC filtering is output in dB. |
| [`SoundLevelResultType`](soundlevelresulttype.md) | Determines the form in which the result of the sound level calculation is output. |
| [`SoundLevelTimeWeighting`](soundleveltimeweighting.md) | Determines the time constant for the time weighting of a sound level. |
| [`SoundType`](soundtype.md) | Specifies the type of sound. |
| [`SourceChn`](sourcechn.md) | Specifies the input channel. |
| [`SourceChnIndex`](sourcechnindex.md) |  |
| [`SourceDateTime`](sourcedatetime.md) | Specifies the time to convert. DIAdem automatically specifies the data type of the time to be converted. It can be the same data type as one of the data types specified in TargetType . Use the ApplicationTimebaseHighResolution variable to resolve DIAdem time data. |
| [`SourceGroupIndex`](sourcegroupindex.md) | Specifies the index of a channel group in the Data Portal. |
| [`SourceUnit`](sourceunit.md) | Specifies the symbol of the source unit. |
| [`SourceUnit1`](sourceunit1.md) | Specifies the symbol of the second source unit. |
| [`SPCCp`](spccp.md) | Receives the process capability index C p . |
| [`SPCCpk`](spccpk.md) | Receives the process capability index C pk . |
| [`SPCCpL`](spccpl.md) | Receives the one-sided lower process capability index C pL . |
| [`SPCCpU`](spccpu.md) | Receives the one-sided upper process capability index C pU . |
| [`SPCFracNConf`](spcfracnconf.md) | Receives the estimated fraction nonconforming in ppm based on a normal process distribution. |
| [`SPCLFracNConf`](spclfracnconf.md) | Receives the estimated fraction nonconforming in ppm below the lower spec limit based on a normal process distribution. |
| [`SPCLowerNPL`](spclowernpl.md) | Receives the lower natural process limit of a process. |
| [`SPCLSL`](spclsl.md) | Specifies the lower specification limit of a process. |
| [`SPCMovingRangeNo`](spcmovingrangeno.md) | Specifies the number of samples that are to be included in the moving range if the sample size is 1, which means the channels with length 1. |
| [`SPCProcessMean`](spcprocessmean.md) | Receives the mean value of a process. |
| [`SPCProcessSigma`](spcprocesssigma.md) | Receives the standard deviation (sigma) of a process. |
| [`SPCSigmaMult`](spcsigmamult.md) | Specifies the sigma multiplier for calculating the upper and the lower natural process limits. |
| [`SPCSigmaTol`](spcsigmatol.md) | Specifies the sigma multiplier for calculating the process capability index. |
| [`SPCSigmaType`](spcsigmatype.md) | Specifies which method to use for calculating the process sigma. |
| [`SPCUFracNConf`](spcufracnconf.md) | Receives the estimated fraction nonconforming in ppm above the upper spec limit based on a normal process distribution. |
| [`SPCUpperNPL`](spcuppernpl.md) | Receives the upper natural process limit of a process. |
| [`SPCUSL`](spcusl.md) | Specifies the upper specification limit of a process. |
| [`SplineParaType`](splineparatype.md) | Specifies the type of spline function. |
| [`SplineType`](splinetype.md) | Specifies the function setup for the spline function. |
| [`SplineWeight`](splineweight.md) | Specifies the weighting factor that affects the overshoot behavior in approximating splines and rational splines. |
| [`SplineXChnType`](splinexchntype.md) | Specifies which method DIAdem uses to generate the interpolation point channel. |
| [`SplineXChnType2`](splinexchntype2.md) | Specifies which method DIAdem uses to generate the interpolation point channel. |
| [`SplineXDiv`](splinexdiv.md) | Specifies the number of partitions in each interval of the x-range. |
| [`SplineXNo`](splinexno.md) | Specifies the number of partitions in the entire x-range. |
| [`SplitValue`](splitvalue.md) | Specifies the limit value at which DIAdem divides a channel. The default setting is 0 . |
| [`SrcVariant`](srcvariant.md) | Specifies the name of the variant that DIAdem converts into channels. |
| [`SRSAmplitudeType`](srsamplitudetype.md) | Specifies the amplitude type of the shock response spectrum. |
| [`SRSDamping`](srsdamping.md) | Specifies the damping degree of the single-degree-of-freedom systems. |
| [`SRSEndFrequency`](srsendfrequency.md) | Specifies the end frequency of the shock response spectrum. |
| [`SRSFreqPerOctave`](srsfreqperoctave.md) | Specifies the number of frequencies per octave of the shock response spectrum. |
| [`SRSPulseDuration`](srspulseduration.md) | Specifies the pulse duration of the shock response. If you specify 0 , the pulse duration is valid for the entire measurement. |
| [`SRSRangeType`](srsrangetype.md) | Specifies the time domain of the shock event. The start range extends over the pulse duration of the shock event. |
| [`SRSResultType`](srsresulttype.md) | Specifies the result type of the shock response spectrum. |
| [`SRSStartFrequency`](srsstartfrequency.md) | Specifies the start frequency of the shock response spectrum. |
| [`SRTMAreaNotSupported`](srtmareanotsupported.md) | Receives the information on whether SRTM data is available for the specified area. |
| [`SRTMLowerLatitudeBound`](srtmlowerlatitudebound.md) | Specifies the lower latitude limit. |
| [`SRTMLowerLongitudeBound`](srtmlowerlongitudebound.md) | Specifies the lower longitude limit. |
| [`SRTMMegaBytesOnDisk`](srtmmegabytesondisk.md) | Receives the information on how many MB on the hard disk are occupied by the downloaded area. |
| [`SRTMMegaBytesToDownload`](srtmmegabytestodownload.md) | Receives the information on how many MB are necessary to download the tiles of the specified area. |
| [`SRTMPassword`](srtmpassword.md) | Specifies the password required for downloading SRTM data from the Earth Observing System Data and Information System (EOSDIS). If you do not have access, you can register at  https://urs.earthdata.nasa.gov/users/new. |
| [`SRTMTilesAvailable`](srtmtilesavailable.md) | Receives the information on how many tiles are available online within the specified area. |
| [`SRTMTilesCacheFolder`](srtmtilescachefolder.md) | Specifies the folder where DIAdem buffers the SRTM data. The path is based on the path you defined in the variable SharedDataPath . If you change this path, you must download all data again. |
| [`SRTMTilesMissing`](srtmtilesmissing.md) | Receives the information on how many tiles are not available online within the specified area. |
| [`SRTMTilesToDownload`](srtmtilestodownload.md) | Receives the information on how many tiles within the specified area DIAdem still must download. |
| [`SRTMUpperLatitudeBound`](srtmupperlatitudebound.md) | Specifies the upper latitude limit. |
| [`SRTMUpperLongitudeBound`](srtmupperlongitudebound.md) | Specifies the upper longitude limit. |
| [`SRTMUsername`](srtmusername.md) | Specifies the user name required for downloading SRTM data from the Earth Observing System Data and Information System (EOSDIS). If you do not have access, you can register at  https://urs.earthdata.nasa.gov/users/new. |
| [`SrvCnfLibrPath`](srvcnflibrpath.md) | Specifies the current library path for TDM Server configuration files, such as search queries or configurations for the file import. |
| [`SrvCnfReadPath`](srvcnfreadpath.md) | Specifies the current write path for TDM Server configuration files, such as search queries or configurations for the file import. |
| [`SrvCnfWritePath`](srvcnfwritepath.md) | Specifies the current write path for TDM Server configuration files, such as search queries or configurations for the file import. |
| [`StatArithMean`](statarithmean.md) |  |
| [`StatAvDevMean`](statavdevmean.md) |  |
| [`StatAvDevMedian`](statavdevmedian.md) |  |
| [`StatCharacter`](statcharacter.md) |  |
| [`StatClipCopy`](statclipcopy.md) |  |
| [`StatClipValue`](statclipvalue.md) |  |
| [`Statdeviation`](statdeviation.md) |  |
| [`Statement`](statement.md) | Specifies a statement that DIAdem executes. |
| [`StatementResult`](statementresult.md) | Specifies the result of a script expression or a statement. |
| [`StatFormat`](statformat.md) |  |
| [`StatFormat2`](statformat2.md) |  |
| [`StatGeoMean`](statgeomean.md) |  |
| [`StatHarMean`](statharmean.md) |  |
| [`StatKey`](statkey.md) |  |
| [`StatKurtosis`](statkurtosis.md) |  |
| [`StatLowerQuartile`](statlowerquartile.md) |  |
| [`StatLowQuantil`](statlowquantil.md) |  |
| [`StatMax`](statmax.md) |  |
| [`StatMedian`](statmedian.md) |  |
| [`StatMin`](statmin.md) |  |
| [`StatOrient`](statorient.md) | Valid names: StatOrient, StatDirec |
| [`StatQuartilDist`](statquartildist.md) |  |
| [`StatRange`](statrange.md) |  |
| [`StatRelVarCoeff`](statrelvarcoeff.md) |  |
| [`StatResChn`](statreschn.md) |  |
| [`StatResChnNameFormat`](statreschnnameformat.md) |  |
| [`StatResChnNames`](statreschnnames.md) |  |
| [`StatSel`](statsel.md) | Specifies which statistical characteristic values to calculate. |
| [`StatSkew`](statskew.md) |  |
| [`StatsPropertyName`](statspropertyname.md) | Specifies the name of the custom properties for the statistical values calculated by the commands ChnStatisticsBlockCalc and ChnStatisticsChannelCalc . |
| [`StatSqrMean`](statsqrmean.md) |  |
| [`StatsResult`](statsresult.md) | Specifies the values of the custom properties for the statistical values calculated by the commands ChnStatisticsBlockCalc and ChnStatisticsChannelCalc . |
| [`StatsResultChn`](statsresultchn.md) | Specifies whether DIAdem stores the statistics results in data channels. |
| [`StatsResultChnNameFormat`](statsresultchnnameformat.md) | Specifies how DIAdem stores the input channel names of the descriptive statistics in a text channel. |
| [`StatsResultChnNames`](statsresultchnnames.md) | Specifies whether DIAdem stores the input channel names of the descriptive statistics in a text channel. |
| [`StatsSelection`](statsselection.md) | Specifies which statistical characteristic values to calculate. |
| [`StatStdError`](statstderror.md) |  |
| [`StatSum`](statsum.md) |  |
| [`StatSumSqr`](statsumsqr.md) |  |
| [`StatsUsePopulationFormula`](statsusepopulationformula.md) | Specifies whether DIAdem calculates the characteristic values based on the population or on the sample. If the value is False , DIAdem calculates the characteristic values based on samples. |
| [`StatTargetChn`](stattargetchn.md) |  |
| [`StatTxt2`](stattxt2.md) |  |
| [`StatUpperQuartile`](statupperquartile.md) |  |
| [`StatUppQuantil`](statuppquantil.md) |  |
| [`StatVarCoeff`](statvarcoeff.md) |  |
| [`Statvariance`](statvariance.md) |  |
| [`StopWatch`](stopwatch.md) | Receives the time that has elapsed since the last start, in seconds. |
| [`StopWatchNo`](stopwatchno.md) | Specifies the number of the time measurement. The default value of the StopWatchNo variable is 0 . |
| [`StorageABS`](storageabs.md) | Specifies a key that you can use to access external data stores. |
| [`SubSequenceText`](subsequencetext.md) | Specifies text for a note that comments a subscript. By default the SubSequenceText variable contains an empty text. |
| [`SUDDlgArgument`](suddlgargument.md) | Specifies the transfer parameter for a user dialog box. In the SUD editor you use the GetArgument method to access the transfer parameters. The default value of the SUDDlgArgument variable is NULL . |
| [`SUDDlgName`](suddlgname.md) | Specifies the name of a user dialog box to be displayed. |
| [`SUDFileName`](sudfilename.md) | Specifies the name of a SUD file. By default the SUDFileName variable contains an empty text. |
| [`SUDNonModalDlgCount`](sudnonmodaldlgcount.md) | Receives the number of the non-modal user dialog boxes. |
| [`SUDNonModalDlgId`](sudnonmodaldlgid.md) | Specifies the number or the name of a non-modal user dialog box. |
| [`SysDrv`](sysdrv.md) | Specifies the folder where DIAdem searches for run-time critical files. When DIAdem is installed the system files are in the program folder. |
| [`SystemInfo`](systeminfo.md) | The SystemInfo object provides information about your system. |
| [`SystemLink`](systemlink.md) | Contains the SystemLink object. |
| [`T1`](t1.md) | Specifies a freely usable text. |
| [`T10`](t10.md) | Specifies a freely usable text. |
| [`T2`](t2.md) | Specifies a freely usable text. |
| [`T3`](t3.md) | Specifies a freely usable text. |
| [`T4`](t4.md) | Specifies a freely usable text. |
| [`T5`](t5.md) | Specifies a freely usable text. |
| [`T6`](t6.md) | Specifies a freely usable text. |
| [`T7`](t7.md) | Specifies a freely usable text. |
| [`T8`](t8.md) | Specifies a freely usable text. |
| [`T9`](t9.md) | Specifies a freely usable text. |
| [`TargetChn`](targetchn.md) | Specifies the target channel. |
| [`TargetChnIndex`](targetchnindex.md) | Specifies the index in a channel group. The index is the visible position in a channel group in the Data Portal. |
| [`TargetGroupIndex`](targetgroupindex.md) | Specifies the index of a target channel group in the Data Portal. |
| [`TargetLine`](targetline.md) | Specifies the row number in the target channel. |
| [`TargetUnit`](targetunit.md) | Specifies the symbol of the target unit. |
| [`TextAlign1stRow`](textalign1strow.md) |  |
| [`TextAlignActive`](textalignactive.md) |  |
| [`THIVAngle`](thivangle.md) | Specifies the angle between the direction of the vehicle and the vehicle axis at the time of impact, in radians. |
| [`THIVDeltaX`](thivdeltax.md) | Specifies the distance between the theoretical head and the theoretical impact surface in x-direction in meters. |
| [`THIVDeltaY`](thivdeltay.md) | Specifies the distance between the theoretical head and the theoretical impact surface in y-direction in meters. |
| [`THIVDistanceX0`](thivdistancex0.md) | Valid names: THIVDistanceX0, THIVDistance |
| [`THIVDistanceY0`](thivdistancey0.md) | Specifies the distance between the theoretical head and the vehicle center of gravity in meters at the time of the impact. |
| [`THIVFlailSpace`](thivflailspace.md) | Contains the flight distance of the theoretical head. |
| [`THIVTimeFlight`](thivtimeflight.md) | Receives the time of collision of the theoretical head with the theoretical impact surface, in seconds. |
| [`THIVVelocity`](thivvelocity.md) | Receives the impact velocity of the theoretical head in kilometers per hour. |
| [`THIVVersion`](thivversion.md) | Receives the version number of the THIV calculation routine. |
| [`TIFcZ`](tifcz.md) | Specifies the critical compression force Fc in the z-direction in kilonewtons. |
| [`TIMcR`](timcr.md) | Specifies the critical bending moment Mc in newton meters. |
| [`TimeAreaCopyBeg`](timeareacopybeg.md) | Specifies the earlier value of the time domain. |
| [`TimeAreaCopyEnd`](timeareacopyend.md) | Specifies the later value of the time domain. |
| [`TimeAreaCopyVer`](timeareacopyver.md) | Specifies the version number of the calculation routine. |
| [`TimeFormat`](timeformat.md) | Specifies the Format that DIAdem uses if no time format is specified. |
| [`TIRes`](tires.md) | Receives the result of the Tibia Index calculation. |
| [`TITime`](titime.md) | Receives the moment of the calculated Tibia index in seconds. |
| [`TIVersion`](tiversion.md) | Receives the version number of the Tibia Index calculation routine. |
| [`TmpDrv`](tmpdrv.md) | Specifies the general temporary path for DIAdem. |
| [`TransposeMatrix`](transposematrix.md) | Specifies whether DIAdem transposes the matrix, which means DIAdem exchanges the rows and columns. The default value is FALSE which means that DIAdem does not swap the rows and columns. |
| [`TTIRes`](ttires.md) | Receives the result of the TTI calculation. |
| [`TTIVersion`](ttiversion.md) | Receives the version number of the TTI calculation routine. |
| [`TV`](tv.md) | Specifies the contents of the vector auxiliary variable for the text type. |
| [`TxtAng`](txtang.md) |  |
| [`TxtBackColor`](txtbackcolor.md) |  |
| [`TxtBackFMode`](txtbackfmode.md) |  |
| [`TxtBackFVariant`](txtbackfvariant.md) |  |
| [`TxtBackRGB`](txtbackrgb.md) |  |
| [`TxtBackRGB2`](txtbackrgb2.md) |  |
| [`TxtBold`](txtbold.md) | Valid names: TxtBold, TB |
| [`TxtClip`](txtclip.md) |  |
| [`TxtColor`](txtcolor.md) | Valid names: TxtColor, TC |
| [`TxtColorRGB`](txtcolorrgb.md) |  |
| [`TxtFont`](txtfont.md) |  |
| [`TxtFrame`](txtframe.md) | Possible spellings: TxtFrame, TF |
| [`TxtItal`](txtital.md) | Valid names: TxtItal, TI |
| [`TxtPosX`](txtposx.md) |  |
| [`TxtPosY`](txtposy.md) |  |
| [`TxtRelPos`](txtrelpos.md) |  |
| [`TxtSize`](txtsize.md) | Valid names: TxtSize, TS |
| [`TxtStrOut`](txtstrout.md) | Valid names: TxtStrOut, TSO |
| [`TxtTxt`](txttxt.md) |  |
| [`TxtUndl`](txtundl.md) | Valid names: TxtUndl, TU |
| [`UIAutoRefresh`](uiautorefresh.md) | Specifies whether DIAdem informs the Data Portal and the DIAdem VIEW panel about changes to the channel contents or the channel properties while the program is running a script. |
| [`UIAutoRefreshArg`](uiautorefresharg.md) | Specifies whether DIAdem informs the Data Portal and the DIAdem VIEW panel about changes to the channel contents or the channel properties. If the variable has the value TRUE , DIAdem refreshes the Data Portal and the DIAdem VIEW panel. |
| [`UniqueNameSep`](uniquenamesep.md) | Specifies which character DIAdem uses to append an index number to a name, when you assign the name of an existing channel or channel group to a channel or to a channel group. |
| [`UnitCatalog`](unitcatalog.md) | Specifies the UnitCatalog object that provides access to the subobjects, methods, and properties of the unit catalog. |
| [`UnitSet`](unitset.md) | Specifies the unit set. |
| [`UrlDatastring`](urldatastring.md) | Specifies the text to be encoded. |
| [`UrlEscapedDatastring`](urlescapeddatastring.md) | Specifies the text to be decoded |
| [`UseChnXYRelationHandling`](usechnxyrelationhandling.md) | Specifies that DIAdem uses channel references in xy-channels and whether the x-channel is used when copying and moving xy-channels. The default value is TRUE . |
| [`UseGlobTFormat`](useglobtformat.md) | Specifies which time format DIAdem uses for the variables CurrTime and CurrDate . |
| [`UsePropTemplate`](useproptemplate.md) | Specifies whether you define custom properties as a template for a data set, for channel groups, and for channels. When you load new data into the Data Portal or when you create new channel groups or channels, DIAdem adds the custom properties from this template to the data set, to the channel groups, and to the channels respectively. DIAdem generates the custom properties of a template in the data set as soon as you delete the internal data store. |
| [`UserBinVarFile`](userbinvarfile.md) | Specifies the name of a variable collection file. |
| [`UserDefColors`](userdefcolors.md) | Specifies user-defined colors. |
| [`UserDrv`](userdrv.md) |  |
| [`UserVarFile`](uservarfile.md) |  |
| [`UserVarMode`](uservarmode.md) |  |
| [`ValDelOnly`](valdelonly.md) | Specifies whether DIAdem deletes only the channel values or also all properties when deleting all values. The default value is FALSE which specifies that DIAdem also deletes the properties. |
| [`ValNo`](valno.md) | Specifies the number of values in a channel. |
| [`ValOnly`](valonly.md) | Specifies whether DIAdem should overwrite the channel names, the description, and the unit, when the target channel is length zero and the clipboard contains the channel name, the description, and the unit. For example, the DataBlClpCopy command copies the channel name and the unit to the clipboard. The default value is FALSE which specifies that DIAdem overwrites the properties. |
| [`ValueInsert`](valueinsert.md) | Specifies the value that DIAdem inserts. The default value of the ValueInsert variable is 0 . |
| [`ValueOverwrite`](valueoverwrite.md) | Specifies whether DIAdem overwrites existing channel data. The default value is FALSE which specifies that DIAdem does not overwrite the input channels. |
| [`ValueUnit`](valueunit.md) | Specifies the numeric value of which DIAdem converts the unit. |
| [`VarName`](varname.md) | Specifies the name of a global variable. |
| [`VBSProcName`](vbsprocname.md) | Specifies the name of a subroutine. By default the VBSProcName variable contains an empty text. For Python scripts, the command ignores this parameter. |
| [`VCDirective`](vcdirective.md) | Specifies the directive or the law for the VC calculation. |
| [`VCScalefactor`](vcscalefactor.md) | Specifies the scaling factor of the dummy. |
| [`View`](view.md) | Specifies the view object that provides access to the subobjects, methods, and properties in the DIAdem VIEW panel. |
| [`ViewDelMode`](viewdelmode.md) | Specifies whether DIAdem deletes the data or replaces the data with NoValues when you select Remove Data Points on the DIAdem VIEW toolbar. |
| [`ViewFitMode`](viewfitmode.md) | Specifies how DIAdem approximates the area selected with flags when you select Interpolate NoValues on the DIAdem VIEW toolbar. |
| [`VIEWMapUserAttribution`](viewmapuserattribution.md) | Specifies the copyright of the map provider. |
| [`VIEWMapUserMaxZoom`](viewmapusermaxzoom.md) | Specifies the maximum zoom level of the map server. |
| [`VIEWMapUserURL`](viewmapuserurl.md) | Specifies the web address of the map source according to the OpenLayers syntax. You can also define several map servers from the same provider in one array. |
| [`ViewRenderingMode`](viewrenderingmode.md) | Specifies the graphic display quality in DIAdem VIEW. A higher output quality may reduce the display speed. |
| [`ViewSoftwareRendering`](viewsoftwarerendering.md) | Specifies whether DIAdem uses the acceleration capabilities of the video card. If the value is TRUE , the graphics acceleration of the graphics card is disabled. Only disable graphics acceleration if problems with the display occur in 3D models. |
| [`ViewTemplate`](viewtemplate.md) | Specifies the template for a new worksheet in DIAdem VIEW. |
| [`ViewUnitDisplayMode`](viewunitdisplaymode.md) | Specifies the display mode for the unit for axis labels in DIAdem VIEW if the channel has a unit. |
| [`VirFree`](virfree.md) |  |
| [`WeightedRegRes`](weightedregres.md) | Specifies the partial results of weighted regression. |
| [`WEIGHTFILTERTYPE`](weightfiltertype.md) | Specifies the frequency weighted curve of the digital filter. |
| [`WfIncrement`](wfincrement.md) | Specifies the step width of the x-part of the waveform channel. |
| [`WfStartOffset`](wfstartoffset.md) | Specifies the offset of the x-part of the waveform channel. |
| [`WfStartTime`](wfstarttime.md) | Specifies the start time of the x-part of the waveform channel. The default value is 01/01/1904 00:00:00 |
| [`WfXName`](wfxname.md) | Specifies the name of the x-part of the waveform channel. |
| [`WfXStartTimeMode`](wfxstarttimemode.md) | Specifies the type of time reference when converting numeric channels and waveform channels. |
| [`WfXUnitString`](wfxunitstring.md) | Specifies the unit of the x-part of the waveform channel. |
| [`WinHelpCommand`](winhelpcommand.md) | Specifies the type of search term. |
| [`WizName`](wizname.md) | Specifies the name of a wizard. |
| [`WizPageName`](wizpagename.md) | Specifies the start page for a wizard. |
| [`WizParam`](wizparam.md) | Specifies further parameters of a wizard. |
| [`WndMode`](wndmode.md) | Specifies the display mode for a DIAdem panel. |
| [`WndName`](wndname.md) | Specifies the name of a DIAdem panel. By default the WndName variable contains the name of the DIAdem panel which was used last. |
| [`WriteWithOutAsk`](writewithoutask.md) | Specifies whether you can overwrite a file without a confirmation prompt. |
| [`XChnDelete`](xchndelete.md) | Specifies whether DIAdem deletes the x-channel after the operation. The default value is FALSE which means that DIAdem does not delete the x-channel. |
| [`XChnNo`](xchnno.md) |  |
| [`XChnStyle`](xchnstyle.md) | Specifies which method DIAdem uses to generate the interpolation point channel. |
| [`XChnStylePara`](xchnstylepara.md) | Specifies which method DIAdem uses to generate the interpolation point channel. |
| [`XDiv`](xdiv.md) | Specifies the number of equidistant sections in each interval of the x-range. |
| [`XgDeltaX`](xgdeltax.md) | Receives the determined time T in the Xg calculation. |
| [`XgMaxPeak`](xgmaxpeak.md) | Receives the time interval between T1 and T2 for the Xg calculation. |
| [`XgRes`](xgres.md) | Specifies the acceleration in gn (gravity acceleration). |
| [`XgTimeBegin`](xgtimebegin.md) | Receives the time T1 of the calculated Xg acceleration. |
| [`XgTimeEnd`](xgtimeend.md) | Receives the time T2 of the calculated Xg acceleration. |
| [`XgType`](xgtype.md) | Specifies whether DIAdem calculates the acceleration, which lasts X ms, from one section or several partial sections. |
| [`XGVersion`](xgversion.md) | Receives the version number of the Xg calculation routine. |
| [`XmsAcceleration`](xmsacceleration.md) | Receives the acceleration of the X ms calculation. |
| [`XmsDeltaX`](xmsdeltax.md) | Receives the determined time T in the Xms calculation. |
| [`XmsNegSigValCalc`](xmsnegsigvalcalc.md) | Specifies whether DIAdem includes the negative signal sections in the X ms calculation. The default value is FALSE which specifies that DIAdem does not consider the negative signal parts. |
| [`XmsRes`](xmsres.md) | Specifies the time X in milliseconds. |
| [`XmsTimeBegin`](xmstimebegin.md) | Receives the time T1 of the calculated Xms acceleration. |
| [`XmsTimeEnd`](xmstimeend.md) | Receives the time T2 of the calculated Xms acceleration. |
| [`XmsType`](xmstype.md) | Specifies whether DIAdem calculates the acceleration from one section or several sections. The default value of the XMSType variable is in one peak . |
| [`XMSVersion`](xmsversion.md) | Receives the version number of the X ms calculation routine. |
| [`XNo`](xno.md) | Specifies the number of values in a new data channel. |
| [`XOffset`](xoffset.md) | Specifies the offset for the first synchronization channel. |
| [`XOffset1`](xoffset1.md) | Specifies the offset for the second synchronization channel. |
| [`XOffset2`](xoffset2.md) | Specifies the offset for the third synchronization channel. |
| [`XOffsetCorrCoefficient`](xoffsetcorrcoefficient.md) | Receives the coefficients of the cross correlation. |
| [`XOffsetCorrCoefficients`](xoffsetcorrcoefficients.md) | Receives the coefficients of the cross correlation. |
| [`XOffsetDeltaN`](xoffsetdeltan.md) | Receives in a cross correlation the number of values of the maximum displacement of the second xy-curve to the first xy-curve. If the XOffsetDeltaN variable receives, for example, the value 4 , you must move the second y-channel up four values in the channel table so that the y-values correspond. |
| [`XOffsetDeltaT`](xoffsetdeltat.md) | Receives in a cross correlation the absolute time value of the maximum offset of the second xy-curve to the first xy-curve. If the XOffsetDeltaT variable receives, for example, the value 4 , you must move the second xy-curve -4 in x-direction so that the y-values correspond. |
| [`XOffsetDeltaTs`](xoffsetdeltats.md) | Receives in an offset calculation the absolute time values of the maximum offset of the second xy-curve to the first xy-curve. If the variable receives, for example, the value 4 , you must move the second xy-curve by -4 in the x-direction so that the y-values correspond. |
| [`XOffsetMode`](xoffsetmode.md) | Specifies whether you set the offset or whether DIAdem automatically sets the offset. |
| [`XOffsetType`](xoffsettype.md) | Specifies whether DIAdem runs a cross correlation calculation in the frequency domain or the time domain. |
| [`XOffsetVal`](xoffsetval.md) | Specifies the maximum shift of the signal, as a percentage of the channel length, for the cross correlation in the time domain. |
| [`XSearchValue`](xsearchvalue.md) | Specifies the x-value of the point which the condition refers to. |
| [`YSearchValue`](ysearchvalue.md) | Specifies the y-value of the point which the condition refers to. |
