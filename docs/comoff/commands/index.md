---
title: "Commands (Commands - Offline (Script Engine))"
---

# Commands

713 commands from `ComOff.chm`.

| Name | Summary |
| --- | --- |
| [`AddUserCommandToEvent`](addusercommandtoevent.md) | Adds a user command to a list of user commands which you assign to an event . If you execute the AddUserCommandToEvent command several times, you can assign several user commands to the same event. |
| [`ADOConStrGet`](adoconstrget.md) | Specifies the ADO connection strings for a database connection via Microsoft-ADO (ActiveX Data Objects) . |
| [`ANALYSISLogClear`](analysislogclear.md) | Deletes the ANALYSIS-Log. |
| [`ANALYSISLogExport`](analysislogexport.md) | Exports the ANALYSIS-Log as HTML file |
| [`ApplicationPreviewFeatureIndexGet`](applicationpreviewfeatureindexget.md) | Specifies the index of a preview feature. |
| [`ApplicationSetLocale`](applicationsetlocale.md) | Switches country specific variables and quantities. The affected variables are TimeFormat and LengthUnit . The paper format and the margins belong to the country specific quantities. If you use the ApplicationSetLocale command in a simulation of the analysis automation or of the data preparation, DIAdem uses the settings only while the script is running. |
| [`ApprAnsatzOff`](appransatzoff.md) | Deletes the selection of all the setup function terms of an approximation. |
| [`AppRectangleGet`](apprectangleget.md) | Specifies the size of a DIAdem window area. DIAdem returns a zero based array which contains the distance in pixels from the left, the upper, the right, and the lower edge to the screen origin. The screen origin is the top-left corner of the screen. |
| [`AppShow`](appshow.md) |  |
| [`ArrayToChannels`](arraytochannels.md) | Converts an array into channels. |
| [`ASCIIBlockLoad`](asciiblockload.md) |  |
| [`AudioOutClose`](audiooutclose.md) | Stops the sound output of channels. |
| [`AudioOutGetSampleRate`](audiooutgetsamplerate.md) | Receives the sampling rate of the audio output. |
| [`AudioOutOpen`](audiooutopen.md) | Starts the audio output of channels. For each audio output you receive as the return value a handle with which you end the audio output via the command AudioOutClose . |
| [`AudioOutResume`](audiooutresume.md) | Continues the audio output. |
| [`AudioOutSetPosition`](audiooutsetposition.md) | Specifies the position of the audio output in the specified play range. |
| [`AudioOutSetRange`](audiooutsetrange.md) | Specifies the first and the last channel value of the audio output. |
| [`AudioOutSetSampleRate`](audiooutsetsamplerate.md) | Specifies the sampling rate of the audio output. |
| [`AudioOutSuspend`](audiooutsuspend.md) | Pauses the audio output. |
| [`AudioOutWaitUntilEnd`](audiooutwaituntilend.md) | Waits until DIAdem finishes the audio output. |
| [`AutEdBPDeleteAll`](autedbpdeleteall.md) |  |
| [`AutEdCloseAll`](autedcloseall.md) | Closes all files in the script editor. DIAdem does not close the current file. |
| [`AutEdEncode`](autedencode.md) | Encrypts VBS files and SUD files. |
| [`AutEdFileNew`](autedfilenew.md) | Creates a new file in the script editor. |
| [`AutEdFileOpen`](autedfileopen.md) | Opens a file in the script editor. |
| [`AutEdInfoGet`](autedinfoget.md) | Provides information about the files loaded in the script editor and the modification status of the files. |
| [`AutEdOpenDlg`](autedopendlg.md) | Opens the load dialog box in the script editor and loads the file that you select in this dialog box. |
| [`AutEdSaveAsDlg`](autedsaveasdlg.md) | Opens the dialog box for saving files in the script editor, without saving the file. |
| [`AutEdTabActivate`](autedtabactivate.md) | Enables a file that is open in the script editor. |
| [`AutEdTabNameGet`](autedtabnameget.md) | Returns the name of a file that is loaded in the script editor. |
| [`AutEdTabSave`](autedtabsave.md) | Saves a file that is open in the script editor. |
| [`AutEdTabTextAdd`](autedtabtextadd.md) |  |
| [`AutEdTypeLibAdd`](autedtypelibadd.md) | Registers a type library to be used in scripts. |
| [`AutEdTypeLibDlg`](autedtypelibdlg.md) | Opens a dialog box for displaying and for selecting the registered type libraries. |
| [`AutEdWSNew`](autedwsnew.md) |  |
| [`AutEdWSOpen`](autedwsopen.md) | Opens a workspace in the DIAdem SCRIPT panel. |
| [`AutEdWSSave`](autedwssave.md) | Saves the current workspace in the DIAdem SCRIPT panel. |
| [`AutEdWSSaveAs`](autedwssaveas.md) | Saves the current workspace with a new name in the DIAdem SCRIPT panel. |
| [`AutoInclude`](autoinclude.md) |  |
| [`AutoLoopInit`](autoloopinit.md) | Starts a progress display in the status bar. |
| [`AutoQuit`](autoquit.md) |  |
| [`AutoRepeat`](autorepeat.md) |  |
| [`Calculate`](calculate.md) | Uses the Calculator formula syntax to calculate a formula in a script including the units. |
| [`CalculatorStart`](calculatorstart.md) | Valid names: CalculatorStart, StartCalculator |
| [`CClassMaxSave`](cclassmaxsave.md) | Calculates compound classification with the maximum value memory method. |
| [`CClassSample`](cclasssample.md) | Calculates compound classification with the sample counting method. |
| [`CClassTimeLev1`](cclasstimelev1.md) | Calculates compound classification with the time-at-level counting method. |
| [`CClassTimeLev2`](cclasstimelev2.md) | Calculates the compound classification with the time-at-level counting method II. |
| [`CClassXRedXY`](cclassxredxy.md) | Classifies a signal and reduces the result data. |
| [`ChannelsToArray`](channelstoarray.md) | Possible spellings: ChannelsToArray, ChnToValue, ChnToVariant |
| [`CharMapDlgShow`](charmapdlgshow.md) | Opens the dialog box of the character table. |
| [`ChnAbsoluteHumidity`](chnabsolutehumidity.md) | Calculates absolute humidity from relative humidity and temperature. |
| [`ChnAccelWCalc`](chnaccelwcalc.md) | Evaluates an acceleration signal with a frequency weighting filter. |
| [`ChnACDCCoupling`](chnacdccoupling.md) | Removes the bias (DAC part) from a signal. DIAdem uses an FFT window function before summating all signal values in order to specify the bias of the signal. DIAdem then subtracts this one value from each value of the input signal. |
| [`ChnACompCalc`](chnacompcalc.md) | Calculates the average acceleration during the compression phase. |
| [`ChnAdd`](chnadd.md) | Adds two or more channels. |
| [`ChnAkimaXYCalc`](chnakimaxycalc.md) | Approximates a signal with an Akima subspline. If required, DIAdem also generates the interpolation points channel necessary for calculating the splines. |
| [`ChnAkimaYCalc`](chnakimaycalc.md) | Approximates a signal with an Akima subspline. |
| [`ChnAlloc`](chnalloc.md) |  |
| [`ChnApprXYCalc`](chnapprxycalc.md) | Approximates a signal. DIAdem also generates the interpolation channel necessary for calculating the approximation. |
| [`ChnApprYCalc`](chnapprycalc.md) | Approximates a signal. |
| [`ChnAreaDel`](chnareadel.md) | Deletes values in a channel. |
| [`ChnAreaInsert0`](chnareainsert0.md) | Inserts data values with zeros into a channel. In the process DIAdem moves existing values down. |
| [`ChnASICalc`](chnasicalc.md) | Calculates the Acceleration Severity Index (ASI). The ASI value determines the effect vehicle acceleration has on a person sitting near a certain point at the time of impact. |
| [`ChnAverage`](chnaverage.md) | Calculates the arithmetic means of the single values of several data channels. |
| [`ChnBrICCalc`](chnbriccalc.md) | Calculates the Rational Brain Injury Criterion values (BrIC). The BRIC value estimates the injury risk of the brain due to rotary movements of the skull. |
| [`ChnCalculate`](chncalculate.md) | Uses the Calculator VBS syntax to calculate a formula in a script. |
| [`ChnCFCFiltCalc`](chncfcfiltcalc.md) | Executes digital phaseless filtering of a signal according to SAE J211. |
| [`ChnCharacter`](chncharacter.md) | Calculates the characteristic values of a channel. |
| [`ChnCharacterAll`](chncharacterall.md) | Calculates the characteristic values of all channels. |
| [`ChnClassLevCross`](chnclasslevcross.md) | Calculates the classification with the level crossing counting method. |
| [`ChnClassMaxMem`](chnclassmaxmem.md) | Calculates the classification with the maximum value memory method. |
| [`ChnClassPeak1`](chnclasspeak1.md) | Calculates the classification with the peak value method I. |
| [`ChnClassPeak2`](chnclasspeak2.md) | Calculates the classification with the peak value method II. |
| [`ChnClassPeak3`](chnclasspeak3.md) | Calculates the classification with the peak value method III. |
| [`ChnClassRange`](chnclassrange.md) | Calculates the classification with the range counting method DIN 45667. |
| [`ChnClassRgPair`](chnclassrgpair.md) | Calculates the range pair classification with a rainflow count. |
| [`ChnClassSample`](chnclasssample.md) | Calculates the classification with the sample counting method DIN 45667. |
| [`ChnClassTimeLev1`](chnclasstimelev1.md) | Calculates the classification with the time-at-level counting method I. |
| [`ChnClassTimeLev2`](chnclasstimelev2.md) | Calculates the classification with the time-at-level counting method II. |
| [`ChnClassXRedXY`](chnclassxredxy.md) | Classifies a signal and reduces the result data. |
| [`ChnClpCopy`](chnclpcopy.md) | Copies channels to the clipboard. |
| [`ChnClpPaste`](chnclppaste.md) | Pastes channels from the clipboard to the default group in the Data Portal. |
| [`ChnConcat`](chnconcat.md) | Possible spellings: ChnConcat, ChnConcatenate |
| [`ChnConcatenateChannels`](chnconcatenatechannels.md) | Concatenates individual channels |
| [`ChnConcatenateGroups`](chnconcatenategroups.md) | Concatenates channels with the same name or the same index of selected groups. |
| [`ChnConcatenateGroupsWithPadding`](chnconcatenategroupswithpadding.md) | Adds all channels from selected groups to the channels of the base group. DIAdem concatenates channels with the same name. To bring all channels to the same length, DIAdem adds NoValues to the channels that are not contained in all groups. |
| [`ChnConvertAssignmentToNumeric`](chnconvertassignmenttonumeric.md) | Valid names: ChnConvertAssignmentToNumeric, AssignmentChnToNumericChn |
| [`ChnConvertAssignmentToText`](chnconvertassignmenttotext.md) | Valid names: ChnConvertAssignmentToText, AssignmentChnToChn |
| [`ChnConvertCartesianToPolar`](chnconvertcartesiantopolar.md) | Valid names: ChnConvertCartesianToPolar, ChnCartesianToPolar |
| [`ChnConvertChannelType`](chnconvertchanneltype.md) | Converts a numeric channel to a complex channel and vice versa. The channel values remain unchanged. |
| [`ChnConvertComplexToNumeric`](chnconvertcomplextonumeric.md) | Creates a numeric channel pair from a complex channel. |
| [`ChnConvertNumericToAssignment`](chnconvertnumerictoassignment.md) | Valid names: ChnConvertNumericToAssignment, ChnToAssignmentChn |
| [`ChnConvertNumericToComplex`](chnconvertnumerictocomplex.md) | Generates a complex channel from a numeric channel pair. |
| [`ChnConvertNumericToTime`](chnconvertnumerictotime.md) | Valid names: ChnConvertNumericToTime, ChnNumericToTime |
| [`ChnConvertNumericToWaveform`](chnconvertnumerictowaveform.md) | Valid names: ChnConvertNumericToWaveform, ChnToWfChn |
| [`ChnConvertPolarToCartesian`](chnconvertpolartocartesian.md) | Valid names: ChnConvertPolarToCartesian, ChnPolarToCartesian |
| [`ChnConvertTextToAssignment`](chnconverttexttoassignment.md) | Valid names: ChnConvertTextToAssignment, TextChnToAssignmentChn |
| [`ChnConvertTimeToNumeric`](chnconverttimetonumeric.md) | Valid names: ChnConvertTimeToNumeric, ChnTimeToNumeric |
| [`ChnConvertUnit`](chnconvertunit.md) | Valid names: ChnConvertUnit, ChnUnitConvert |
| [`ChnConvertUnitToUnitSet`](chnconvertunittounitset.md) | Valid names: ChnConvertUnitToUnitSet, ChnConvertToUnitSet |
| [`ChnConvertWaveformToNumeric`](chnconvertwaveformtonumeric.md) | Valid names: ChnConvertWaveformToNumeric, WfChnToChn |
| [`ChnConvertWaveformXUnit`](chnconvertwaveformxunit.md) | Valid names: ChnConvertWaveformXUnit, ChnWfxUnitConvert |
| [`ChnConvexHull`](chnconvexhull.md) | Calculates the convex hull of a set of points. |
| [`ChnCopy`](chncopy.md) | Copies a channel into another channel. You also can use the object-oriented interface to access internal data. Use Channels . AddChannels from the script interface for internal data to realize the functionality of the ChnCopy command. |
| [`ChnCopyExt`](chncopyext.md) |  |
| [`ChnCorrelAuto`](chncorrelauto.md) | Calculates an autocorrelation. |
| [`ChnCorrelCross`](chncorrelcross.md) | Calculates a cross correlation. |
| [`ChnCorrelNAuto`](chncorrelnauto.md) | Calculates a normalized autocorrelation, which means the result values are between -1 and 1. |
| [`ChnCorrelNCross`](chncorrelncross.md) | Calculates a normalized cross correlation, which means the result values are between -1 and 1. |
| [`ChnCorridor`](chncorridor.md) | Calculates two curves which have a fixed distance to the input signal. All points of the input signal and the connection line between two consecutive points are in the band formed by the result channels. |
| [`ChnCorridorCheck`](chncorridorcheck.md) | Checks whether a signal is in a specified range. |
| [`ChnCWVCalc`](chncwvcalc.md) | Calculates the chest wall velocity that occurs when the chest is crushed by a pressure wave. The chest wall velocity allows statements about injuries to internal organs by overpressure waves which do not affect the ear. |
| [`ChnD3Appr`](chnd3appr.md) | Uses a setup function to approximate a surface for three-dimensional, triplet data. |
| [`ChnD3Interp`](chnd3interp.md) | Calculates a three-dimensional interpolation for a data triplet with x, y and z-channels. |
| [`ChnD3InterpPoint`](chnd3interppoint.md) | Calculates a single z-value of a three-dimensional interpolation for a data triplet with x, y and z-channels. |
| [`ChnDel`](chndel.md) |  |
| [`ChnDelete`](chndelete.md) |  |
| [`ChnDeleteDuplicateTexts`](chndeleteduplicatetexts.md) | Deletes identical texts from a channel. If you specify more dependent channels in ChnList1 , DIAdem also deletes the respective values in these channels. |
| [`ChnDeleteDuplicateValues`](chndeleteduplicatevalues.md) | Deletes equal numeric values form a channel. If you specify more dependent channels in ChnList1 , DIAdem also deletes the respective values in these channels. To determine that two values are identical, the command uses the internal DIAdem algorithm. This algorithm only includes the significant digits of a number. |
| [`ChnDeltaCalc`](chndeltacalc.md) | Calculates the difference between two successive channel values. |
| [`ChnDeriveCalc`](chnderivecalc.md) | Differentiates a signal numerically by calculating the central difference quotient of the second order. |
| [`ChnDetrendCalc`](chndetrendcalc.md) | Removes a trend in the channel data. |
| [`ChnDifferentiate`](chndifferentiate.md) | Differentiates a signal numerically by calculating the forward difference quotient of the first order. |
| [`ChnDiv`](chndiv.md) | Divides two channels. |
| [`ChnDRICalc`](chndricalc.md) | Calculates the Dynamic Response Index value (DRI). The Dynamic Response Index value is a criterion for axial compression force injuries to the thoracic-lumbar spine. The DRI is a dimensionless value related to the spine deflection. |
| [`ChnDurationCalc`](chndurationcalc.md) | Calculates the time at level. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific lower threshold. |
| [`ChnDurInjuryCalc`](chndurinjurycalc.md) | Calculates the time-at-level and the injury risk. The time at level describes the maximum continuous time interval in which the amplitude value of a signal exceeds a specific lower threshold. |
| [`ChnDurPosCalc`](chndurposcalc.md) | Calculates the time at level. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific threshold. |
| [`ChnDurPosInjCalc`](chndurposinjcalc.md) | Calculates the time-at-level and the injury risk for positive limit curves. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific threshold. |
| [`ChnDurPosNegCalc`](chndurposnegcalc.md) | Specifies the time-at-level for positive and for negative values. The time at level describes the maximum continuous time interval in which the amplitude value of a signal exceeds a specific lower threshold. |
| [`ChnDXDivGen`](chndxdivgen.md) | Generates a data channel by partitioning a specific x-channel into equidistant sections. |
| [`ChnEnclosedArea`](chnenclosedarea.md) | Calculates the area between two or more curves or one curve and the x-axis. |
| [`ChnEnvelopes`](chnenvelopes.md) | Calculates the upper and lower envelope curve of a signal. |
| [`ChnEventCompareChnEQ`](chneventcomparechneq.md) | Determines the area in a data channel in which the value is equal to the value of the second channel. |
| [`ChnEventCompareChnGE`](chneventcomparechnge.md) | Determines the area in a data channel in which the value is greater or equal the value of the second channel. |
| [`ChnEventCompareChnGT`](chneventcomparechngt.md) | Determines the area in a data channel in which the value is greater than the value of the second channel. |
| [`ChnEventCompareChnLE`](chneventcomparechnle.md) | Determines the area in a data channel in which the value is less than or equal to the value of the second channel. |
| [`ChnEventCompareChnLT`](chneventcomparechnlt.md) | Determines the area in a data channel in which the value is less than the value of the second channel. |
| [`ChnEventCompareChnNE`](chneventcomparechnne.md) | Determines the area in a data channel in which the value is not equal to the value of the second channel. |
| [`ChnEventCopyValues`](chneventcopyvalues.md) | Copies the values of an event search into new channels. |
| [`ChnEventCount`](chneventcount.md) | Specifies the number of results in an event search. |
| [`ChnEventCreateFilteredChn`](chneventcreatefilteredchn.md) | Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is fulfilled, and otherwise uses the channel values of a second specified channel. |
| [`ChnEventCreateFilteredFalseChn`](chneventcreatefilteredfalsechn.md) | Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is not fulfilled, and otherwise uses a specified value. |
| [`ChnEventCreateFilteredTrueChn`](chneventcreatefilteredtruechn.md) | Generates a result channel from the search results when DIAdem copies the values of a specified channel if the search condition is fulfilled, and otherwise uses a specified value. |
| [`ChnEventCreateStatusChn`](chneventcreatestatuschn.md) | Creates a result channel from the search results. |
| [`ChnEventCreateXYChannels`](chneventcreatexychannels.md) | Specifies whether DIAdem creates a channel with a time channel for each section in which the search condition is met. |
| [`ChnEventDetectionDifference`](chneventdetectiondifference.md) | Checks whether two successive single values differ by a certain amount. |
| [`ChnEventDetectionEqualStr`](chneventdetectionequalstr.md) | Checks whether a character string and a text in a text channel are the same. |
| [`ChnEventDetectionInStr`](chneventdetectioninstr.md) | Checks whether a text in a text channel contains a character string. |
| [`ChnEventDetectionSlope`](chneventdetectionslope.md) | Checks whether the values of a channel exceed a limit value in the specified slope direction. You can search for rising and falling slopes and specify an optional hysteresis range. |
| [`ChnEventDetectionWindow`](chneventdetectionwindow.md) | Checks whether the values of a channel are in a specified window. You can specify an optional hysteresis range for the upper and lower window limit. |
| [`ChnEventDuration`](chneventduration.md) | Specifies the duration of individual events or of all events from the results list of an event search. |
| [`ChnEventFilter`](chneventfilter.md) | Checks whether a search result contains short phases in which an event is fulfilled or not fulfilled, and filters these positive or negative peaks from the search results. |
| [`ChnEventFind`](chneventfind.md) | Determines the area in a data channel that meets a specified condition. |
| [`ChnEventGate`](chneventgate.md) | Connects two search results with the GATE operator. DIAdem interprets the first search result as a list of start events and the second search result as a list of stop events. The ChnEventGateType setting determines whether DIAdem uses the first or last start event as start and ignores all following start and stop events until the first or the last stop event occurs. |
| [`ChnEventInvalidValues`](chneventinvalidvalues.md) | Checks whether a channel contains values (NoValues). |
| [`ChnEventOperationAND`](chneventoperationand.md) | Connects two search results with the AND operator. |
| [`ChnEventOperationEventIncluded`](chneventoperationeventincluded.md) | Connects two search results with the INCLUDE operator. The second search result must be contained in the first search result for the search condition to be valid. |
| [`ChnEventOperationNOT`](chneventoperationnot.md) | Negates a search result with the NOT operator. The length of channel SourceChn specifies the maximum index of the result array. |
| [`ChnEventOperationOR`](chneventoperationor.md) | Connects two search results with the OR operator. |
| [`ChnEventPatternFind`](chneventpatternfind.md) | Searches for a pattern in a signal. |
| [`ChnEventResultAddPrePost`](chneventresultaddprepost.md) | Adds a number of values or a value range at the beginning or the end of a search result. The index of advanced search results is never smaller than one or greater than the channel length of the input channel. If the extended areas of the search results overlap, the command combines these areas to one area. |
| [`ChnEventSampleCount`](chneventsamplecount.md) | Specifies the number of values of an individual event or of all events from the results list of an event search. Use the ChnEventStatValueCount command to count only those values at which the specified channel does not contain any NoValues. |
| [`ChnEventSort`](chneventsort.md) | Sorts the results list of an event search according to its length. |
| [`ChnEventStatArithMean`](chneventstatarithmean.md) | Specifies the arithmetic mean of an individual event or of all events from the results list of an event search. |
| [`ChnEventStatMax`](chneventstatmax.md) | Specifies the maximum value of an individual event or of all events from the result list of an event search. |
| [`ChnEventStatMin`](chneventstatmin.md) | Specifies the minimum value of an individual event or of all events from the result list of an event search. |
| [`ChnEventStatRange`](chneventstatrange.md) | Specifies the span width of an individual event or of all events from the results list of an event search. |
| [`ChnEventStatStandardDeviation`](chneventstatstandarddeviation.md) | Specifies the standard deviation of individual events or of all events from the result list of an event search. |
| [`ChnEventStatSum`](chneventstatsum.md) | Specifies the sum of individual events or of all events from the result list of an event search. |
| [`ChnEventStatValueCount`](chneventstatvaluecount.md) | Specifies the number of values of an individual event or of all events from the results list of an event search. DIAdem only counts the values at which the specified channel does not contain NoValues. Use the ChnEventSampleCount command to also count the number of values of an event irrespective of the values of a channel. |
| [`ChnExpand`](chnexpand.md) |  |
| [`ChnFFCBdryCalc`](chnffcbdrycalc.md) | Calculates the Femur Force Criterion values (FFC). |
| [`ChnFFCCalc`](chnffccalc.md) | Calculates the Femur Force Criterion values (FFC), which is the force on the femur. |
| [`ChnFFT1`](chnfft1.md) | Executes a fast Fourier transform (FFT) of a signal. |
| [`ChnFFT2`](chnfft2.md) | Executes a fast Fourier transform (FFT) of two signals with a common time channel. |
| [`ChnFiltCalc`](chnfiltcalc.md) | Filters a signal digitally. |
| [`ChnFind`](chnfind.md) | Determines the first row in a data channel that meets a specified condition. The ChnFind function searches a data channel from the beginning to the end. |
| [`ChnFindReverse`](chnfindreverse.md) | Determines the first row in a data channel that meets a specified condition. The ChnFindReverse function searches a data channel from the end to the beginning. |
| [`ChnFindXYValue`](chnfindxyvalue.md) | Specifies for an x/y-coordinate the point on a curve that corresponds to either the next value, the interpolated value, or a maximum or a minimum. The command specifies the row number of a channel pair whose values meet the specified condition. You can specify the 3D data as a triplet or as a matrix. |
| [`ChnFindXYZValue`](chnfindxyzvalue.md) | Specifies for an x/y-coordinate the x/y/z-values on a surface that either correspond to the next value on the surface, the interpolated surface value, or the maximum or the minimum of the surface. This command specifies the rows of the x-channel and the y-channel, the values of which meet the given condition. You can specify the 3D data as a triplet or as a matrix. |
| [`ChnFIR100Calc`](chnfir100calc.md) | Use this command for digital signal filtering. |
| [`ChnFlagDel`](chnflagdel.md) | Deletes all the Flags of a channel. |
| [`ChnFlagDelAll`](chnflagdelall.md) | Deletes the Flags of all channels. |
| [`ChnFlagSet`](chnflagset.md) | Sets Flags for several successive values of a channel. |
| [`ChnFromWfXGen`](chnfromwfxgen.md) | Generates a data channel from the x-part of a specified waveform channel. |
| [`ChnFullSpectrum`](chnfullspectrum.md) | Calculates the full spectrum for a vibration analysis. |
| [`ChnGaussFitXY`](chngaussfitxy.md) | Calculates a Gaussian curve fitting with the least square method, the least residual method, or the bisquare method. If required, DIAdem also generates the interpolation points channel necessary for the calculation. |
| [`ChnGaussFitXYWeighted`](chngaussfitxyweighted.md) | Calculates a Gaussian curve fitting with the least square method, the least residual method, or the bisquare method. DIAdem includes the y-channel weightings. If required, DIAdem also generates the interpolation points channel necessary for the calculation. |
| [`ChnGaussFitY`](chngaussfity.md) | Calculates a Gaussian curve fitting with the least square method, the least residual method, or the bisquare method. |
| [`ChnGaussFitYWeighted`](chngaussfityweighted.md) | Calculates a Gaussian curve fitting with the least square method, the least residual method, or the bisquare method. DIAdem includes the y-channel weightings. |
| [`ChnGenLSFit`](chngenlsfit.md) | Specifies the k-dimensional linear curve values and the k-dimensional coefficients for linear fitting that best fit a k-dimensional curve using the least square method. |
| [`ChnGenLSFitWeighted`](chngenlsfitweighted.md) | Specifies the k-dimensional linear curve values and the k-dimensional coefficients for linear fitting that best fit a k-dimensional curve using the least square method. DIAdem includes the y-channel weightings. |
| [`ChnGenSignal`](chngensignal.md) | Generates a new channel with a given signal form. |
| [`ChnGenTime`](chngentime.md) | Generates a time channel with equidistant values. |
| [`ChnGenVal`](chngenval.md) | Generates a data channel with equidistant values. |
| [`ChnGeoGen`](chngeogen.md) | Generates a data channel with geometric partitions. |
| [`ChnGPSDistanceFromStart`](chngpsdistancefromstart.md) | Calculates the shortest distance of the first coordinate to the following coordinates considering the ellipsoidal shape of the Earth. The function sums up the values. |
| [`ChnHCDCalc`](chnhcdcalc.md) | Calculates the Head Contact Duration values (HCD). The HCD value is a normalized maximum integral value of the head acceleration. |
| [`ChnHICCalc`](chnhiccalc.md) | Calculates the Head Injury Criterion values (HIC). The HIC value is a normalized maximum integral value of the head acceleration. |
| [`ChnHistogram`](chnhistogram.md) | Runs a histogram classification. |
| [`ChnHPCCalc`](chnhpccalc.md) | Calculates the Head Performance Criterion (HPC). The HPC value is a normalized maximum integral value of the head acceleration. |
| [`ChnIntegrate`](chnintegrate.md) | Integrates a signal. |
| [`ChnInverseFFT`](chninversefft.md) | Executes an inverse fast Fourier transform (FFT). DIAdem transforms a signal from the frequency domain into the time domain. |
| [`ChnInvert`](chninvert.md) | Mirrors the values in a data channel. DIAdem exchanges the first channel value with the last value and so on. |
| [`ChnIsEquidistant`](chnisequidistant.md) | Specifies whether a channel is equidistant. |
| [`ChnIsolinesCalc`](chnisolinescalc.md) | Calculates contour lines on a surface with a triplet structure. |
| [`ChnKFiltCalc`](chnkfiltcalc.md) | Analyzes mechanical vibrations that effect the human body in manifold ways, for example, at the workplace or in vehicles. |
| [`ChnKTHCalc`](chnkthcalc.md) | Calculates the Knee Thigh Hip (KTH) value, which represents the risk of injury to the hip and thigh. |
| [`ChnLateralAbdominalRibDisplacement`](chnlateralabdominalribdisplacement.md) | Calculates the Lateral Abdominal Rib Displacement value which is a criteria for the lateral shift of the abdominal ribs. |
| [`ChnLateralShoulderRibDisplacement`](chnlateralshoulderribdisplacement.md) | Calculates the Lateral Shoulder Rib Displacement value which is a criteria for the lateral shift of the shoulder ribs. |
| [`ChnLateralThoracicRibDisplacement`](chnlateralthoracicribdisplacement.md) | Calculates the Lateral Thoracic Rib Displacement value which is a criteria for the lateral shift of the chest ribs. |
| [`ChnLinGen`](chnlingen.md) | Generates a data channel with equidistant values. |
| [`ChnLinGenImp`](chnlingenimp.md) | Generates an implicit channel with a prescribed linear generation. |
| [`ChnLinScale`](chnlinscale.md) | Scales a channel. |
| [`ChnListToChnStr`](chnlisttochnstr.md) |  |
| [`ChnLower`](chnlower.md) | Converts letters in a text channel into lowercase letters. |
| [`ChnMapLinCalc`](chnmaplincalc.md) | Maps a signal onto a new x-range. |
| [`ChnMapLinCalcExt`](chnmaplincalcext.md) | Maps several signals onto a new common x-value range. |
| [`ChnMatConvert`](chnmatconvert.md) | Converts a data triplet from an x, y and z-channel into a matrix structure. |
| [`ChnMirror`](chnmirror.md) | Mirrors the data in a channel so that the last channel value comes first. |
| [`ChnMove`](chnmove.md) |  |
| [`ChnMul`](chnmul.md) | Multiplies two or more channels. |
| [`ChnMultipleSort`](chnmultiplesort.md) | Sorts values in data channels in ascending order. DIAdem sorts texts according to the ASCII table. |
| [`ChnMultipleSortExt`](chnmultiplesortext.md) | Sorts the values in data channels. DIAdem sorts texts according to the ASCII table. |
| [`ChnNameChk`](chnnamechk.md) |  |
| [`ChnNConvexHull`](chnnconvexhull.md) | Calculates the non-convex hull of a set of points. |
| [`ChnNICBdryCalc`](chnnicbdrycalc.md) | Calculates the Neck Injury Criterion value (NIC) according to ECE. |
| [`ChnNICCalc`](chnniccalc.md) | Calculates the Neck Injury Criterion value (NIC) according to ECE. |
| [`ChnNICRearCalc`](chnnicrearcalc.md) | Calculates the Neck Injury Criterion Rear Impact. |
| [`ChnNijCalc`](chnnijcalc.md) | Calculates the Normalized Neck Injury Criterion value (Nij) according to FMVSS. |
| [`ChnNijCalcAll`](chnnijcalcall.md) | Simultaneously calculates the Normalized Neck Injury Criterion value (Nij) according to FMVSS for all four calculation types (NTE, NTF, NCE and NCF). |
| [`ChnNonLinearFitXY`](chnnonlinearfitxy.md) | Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non-linear function of the y = f(x,a) type. If required, DIAdem also generates the interpolation points channel necessary for the calculation. |
| [`ChnNonLinearFitXYWeighted`](chnnonlinearfitxyweighted.md) | Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non-linear function of the y = f(x,a) type. If required, DIAdem also generates the interpolation points channel necessary for the calculation. DIAdem includes the y-channel weightings. If required, DIAdem also generates the interpolation points channel necessary for the calculation. |
| [`ChnNonLinearFitY`](chnnonlinearfity.md) | Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non-linear function of the y = f(x,a) type. |
| [`ChnNonLinearFitYWeighted`](chnnonlinearfityweighted.md) | Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non-linear function of the y = f(x,a) type. If required, DIAdem also generates the interpolation points channel necessary for the calculation. DIAdem includes the y-channel weightings. |
| [`ChnNormalize`](chnnormalize.md) | Normalizes a data channel to the value one. |
| [`ChnNovHandle`](chnnovhandle.md) | Removes or interpolates NoValues in data channels. |
| [`ChnOffset`](chnoffset.md) | Subtracts an offset from the channel values or adds an offset to the channel values. |
| [`ChnOIVCalc`](chnoivcalc.md) | Calculates the Occupant Impact Velocity (OIV). |
| [`ChnOptimizeDataType`](chnoptimizedatatype.md) | Optimizes the data type of a channel to save disk space. |
| [`ChnORACalc`](chnoracalc.md) | Calculates the Occupant Ridedown Acceleration (ORA). |
| [`ChnOrdAFCalc`](chnordafcalc.md) | Calculates an order analysis in the frequency domain. |
| [`ChnOrdATCalc`](chnordatcalc.md) | Runs an order and frequency analysis in the time domain of a signal. |
| [`ChnOrderBodeCalc`](chnorderbodecalc.md) | Uses the sensor signals to calculate the amplitudes and phases for each order for a Bode diagram. |
| [`ChnPeakDetect`](chnpeakdetect.md) | Executes a peak value recognition, which means that DIAdem specifies the position, the second deduction, and the amplitude of the peaks and valleys in the input signal. |
| [`ChnPeakFind`](chnpeakfind.md) | Determines the local minimum and maximum values in a signal. |
| [`ChnPhaseUnwrap`](chnphaseunwrap.md) | Unwraps phases in a channel. |
| [`ChnPhaseWrap`](chnphasewrap.md) | Wraps phases in a channel. |
| [`ChnPHDCalc`](chnphdcalc.md) | Calculates the Post Impact Head Deceleration (PHD). |
| [`ChnPropCopy`](chnpropcopy.md) | Copies all channel properties to another channel. You also can use the object-oriented interface to access internal data. Use the AddProperties for Properties to implement the functionality of the ChnPropCopy command with the script interface for internal data. |
| [`ChnPropCreate`](chnpropcreate.md) |  |
| [`ChnPropDel`](chnpropdel.md) |  |
| [`ChnPropExist`](chnpropexist.md) |  |
| [`ChnPropInfoGet`](chnpropinfoget.md) |  |
| [`ChnPropNameChk`](chnpropnamechk.md) |  |
| [`ChnPropSet`](chnpropset.md) |  |
| [`ChnPropValGet`](chnpropvalget.md) |  |
| [`ChnPropValSet`](chnpropvalset.md) |  |
| [`ChnPulseDetection`](chnpulsedetection.md) | Evaluates the tachometer signals. At regular intervals a tachometer signal contains pulses measured by sensors on a shaft. |
| [`ChnPulseLimit`](chnpulselimit.md) | Checks whether acceleration values are in a specified range. |
| [`ChnQuantize`](chnquantize.md) | Maps the values of a channel in quantization steps. |
| [`ChnRainCalc`](chnraincalc.md) | Calculates the rainflow classification. |
| [`ChnRangeLimit`](chnrangelimit.md) | Restricts a data channel to the values between an upper and lower limit value. DIAdem replaces the values outside the value range with the upper or lower limit value. |
| [`ChnReAlloc`](chnrealloc.md) |  |
| [`ChnReciprocal`](chnreciprocal.md) | Calculates the reciprocal value of a channel. |
| [`ChnRegrXYCalc`](chnregrxycalc.md) | Uses a regression function to approximate a signal. If required, DIAdem also generates the interpolation points channel necessary for calculating the regression. |
| [`ChnRegrYCalc`](chnregrycalc.md) | Uses a regression function to approximate a signal. |
| [`ChnRelativeHumidity`](chnrelativehumidity.md) | Calculates relative humidity from absolute humidity and temperature. |
| [`ChnRelativize`](chnrelativize.md) | Determines for each channel value the percentage of the total sum of all channel values. |
| [`ChnRenumber`](chnrenumber.md) | Renumbers channels. DIAdem numbers the channels starting from 1 in ascending order, according to the Data Portal structure view. |
| [`ChnResampleChnBased`](chnresamplechnbased.md) | Maps a signal onto an interpolation channel. |
| [`ChnResampleChnBasedExt`](chnresamplechnbasedext.md) | Maps several signals onto a common interpolation channel. |
| [`ChnResampleChnBasedXOffsetCalc2`](chnresamplechnbasedxoffsetcalc2.md) | Uses a synchronization channel to map two measurements onto new interpolation channels. |
| [`ChnResampleChnBasedXOffsetCalc3`](chnresamplechnbasedxoffsetcalc3.md) | Uses a synchronization channel to map three measurements onto new interpolation channels. |
| [`ChnResampleFreqBased`](chnresamplefreqbased.md) | Maps a signal onto a new sampling rate. |
| [`ChnResampleFreqBasedExt`](chnresamplefreqbasedext.md) | Maps several signals onto a common sampling rate. |
| [`ChnResampleFreqBasedXOffsetCalc2`](chnresamplefreqbasedxoffsetcalc2.md) | Uses a synchronization channel to map two measurements on a new sampling rate. |
| [`ChnResampleFreqBasedXOffsetCalc3`](chnresamplefreqbasedxoffsetcalc3.md) | Uses a synchronization channel to map three measurements on a new sampling rate. |
| [`ChnResultUnitGet`](chnresultunitget.md) | Returns the symbol of the result unit if you perform an arithmetic operation on a channel. |
| [`ChnRMS`](chnrms.md) | Calculates floating root mean squares, RMS. |
| [`ChnRound`](chnround.md) | Rounds a channel. |
| [`ChnSavitzkyGolayFilter`](chnsavitzkygolayfilter.md) | Smoothes a data channel with the Savitzky-Golay filter. |
| [`ChnSavitzkyGolayFilterWeighted`](chnsavitzkygolayfilterweighted.md) | Uses weighting factors to smooth a data channel with the Savitzky-Golay filter. |
| [`ChnSDel`](chnsdel.md) |  |
| [`ChnSeismicPhasePicking`](chnseismicphasepicking.md) | Specifies the arrival times of the primary waves (P waves) and the secondary waves (S waves) of a seismic event. DIAdem calculates P-waves with the moving averages short-term average (STA) and long-term average (LTA). |
| [`ChnShaftCenterline`](chnshaftcenterline.md) | Calculates the movement of a rotating shaft over an extended time period. The measurement values of two sensors at the shaft are averaged in order to specify how the position of the shaft center changes over several revolutions. |
| [`ChnShockResponseSpectrum`](chnshockresponsespectrum.md) | Calculates the shock response spectrum (SRS) from an acceleration signal. The calculation is executed in accordance with ISO-Norm 18431-4:2007. The shock response spectrum describes the response to the acceleration of many single-degree-of-freedom systems which is a mass-damping-spring system with different natural harmonics. |
| [`ChnSICalc`](chnsicalc.md) | Calculates the Severity Index (SI) which is an injury criterion for the chest and rib area. |
| [`ChnSINAD`](chnsinad.md) | Executes a SINAD analysis (Signal to Noise and Distortion) which specifies the signal-noise interval plus the distortion of a signal. The command determines the basic oscillation and outputs the basic frequency and the SINAD value in decibel. |
| [`ChnSingleToneExtract`](chnsingletoneextract.md) | Specifies the single frequency with the greatest amplitude in the input signal and returns the frequency and the associated amplitude and phase. |
| [`ChnSmooth`](chnsmooth.md) | Uses the floating arithmetic mean or the floating median to smooth a data channel. |
| [`ChnSmooth4253H`](chnsmooth4253h.md) | Smoothes a data channel using the 4253H filter. |
| [`ChnSoundLevelAverage`](chnsoundlevelaverage.md) | Calculation of a time-weighted sound level |
| [`ChnSplinePara`](chnsplinepara.md) | Uses a parametrical spline to approximate a signal. |
| [`ChnSplineXYCalc`](chnsplinexycalc.md) | Uses a non-parametrical spline to approximate a signal. If required, DIAdem also generates the interpolation points channel necessary for calculating the splines. |
| [`ChnSplineYCalc`](chnsplineycalc.md) | Uses a non-parametrical spline to approximate a signal. |
| [`ChnSplitAtValue`](chnsplitatvalue.md) | Splits a channel into two new channels at a specified limit value. |
| [`ChnSRTMAltitude`](chnsrtmaltitude.md) | Determines the corresponding elevation values from the latitudes and longitudes. Before calling this function, you must download the appropriate SRTM data into the cache folder using the SRTMDownloadTilesArea function. |
| [`ChnStatisticsBlockCalc`](chnstatisticsblockcalc.md) | Calculates characteristic statistical values rowwise. |
| [`ChnStatisticsChannelCalc`](chnstatisticschannelcalc.md) | Calculates characteristic statistical values channelwise. |
| [`ChnStatisticsMovingWindow`](chnstatisticsmovingwindow.md) | Calculates statistical characteristic values channel by channel, whereby the characteristic values are calculated through a symmetrical window that is moved across the channel values. If the window size is even, the portion of the window before the current channel value is one value larger than after the current channel value. If there are not enough elements at the endpoints, DIAdem will automatically cut off the window. |
| [`ChnStatisticsMovingWindowAsymmetric`](chnstatisticsmovingwindowasymmetric.md) | Calculates statistical characteristic values channel by channel, whereby the characteristic values are calculated through an asymmetrical window that is moved across the channel values. You can separately specify the window size before and after the current channel value. If there are not enough elements at the endpoints, DIAdem will automatically cut off the window. |
| [`ChnSub`](chnsub.md) | Subtracts one channel from another. |
| [`ChnSum`](chnsum.md) | Adds up the single values of the data channel. |
| [`ChnTHIVCalc`](chnthivcalc.md) | Calculates the Theoretical Head Impact Velocity (THIV). |
| [`ChnTICalc`](chnticalc.md) | Calculates the Tibia Index value (TI). This value is an injury criterion for the lower leg. |
| [`ChnTimeAreaCopy`](chntimeareacopy.md) | Copies a time range and the related amplitudes into two new data channels. |
| [`ChnTMinTMaxCalc`](chntmintmaxcalc.md) | Determines the time points of the minimum and maximum values in a signal. |
| [`ChnTTICalc`](chntticalc.md) | Calculates the Thorax Trauma Index (TTI). This value is the injury criterion for the chest area. |
| [`ChnUpper`](chnupper.md) | Converts letters in a text channel into uppercase letters. |
| [`ChnValExpand`](chnvalexpand.md) | Expands registered or implicit channels into standard DIAdem channels. |
| [`ChnVCCalc`](chnvccalc.md) | Calculates the Viscous Criterion value (VC), which is an injury criterion for the chest area. |
| [`ChnWeightFilter`](chnweightfilter.md) | Executes a frequency weighted digital filter. |
| [`ChnWfPropCopy`](chnwfpropcopy.md) | Copies the waveform properties of a waveform channel to another channel. The channel whose waveform properties you want to copy must be a waveform channel. When you convert an xy-channel to a waveform channel, DIAdem automatically removes the xy relationship. |
| [`ChnWfPropSet`](chnwfpropset.md) | Sets the waveform property of channels. If the specified channels are not waveform channels, DIAdem converts the channels into waveform channels. When you convert an xy-channel to a waveform channel, DIAdem automatically removes the xy relationship. |
| [`ChnXGCalc`](chnxgcalc.md) | Determines the total time in milliseconds for which the acceleration signal is x-times gn (gravity acceleration). |
| [`ChnXMSCalc`](chnxmscalc.md) | Determines the maximum acceleration value that lasts at least x milliseconds. |
| [`ChnXYZAbsValue`](chnxyzabsvalue.md) | Calculates the resultant acceleration for an x, y, and z-channel. |
| [`ChVXYValue`](chvxyvalue.md) | Specifies for an x/y-coordinate the point on a curve that corresponds to either the next value, the interpolated value, or a maximum or a minimum. You can specify the 3D data as a triplet or as a matrix. |
| [`ChVXYZValue`](chvxyzvalue.md) | Specifies for an x/y-coordinate the x/y/z-values on a surface that either correspond to the next value on the surface, the interpolated surface value, or the maximum or the minimum of the surface. You can specify the 3D data as a triplet or as a matrix. |
| [`CircleConcCalc`](circleconccalc.md) | Calculates the regression circle, the concentric circumcircle, and the concentric incircle for a point set. |
| [`CircleExtremeCalc`](circleextremecalc.md) | Calculates the regression circle, the minimum circumcircle, and the maximum incircle for a set of points. |
| [`CircleRegrCalc`](circleregrcalc.md) | Calculates the regression circle for a set of points. |
| [`ClpEMFExport`](clpemfexport.md) |  |
| [`ColorChoose`](colorchoose.md) | Opens the dialog box for color selection. |
| [`CommonTimeFormatCheck`](commontimeformatcheck.md) | Checks whether a time format is commonly applicable and specifies a universal format string. |
| [`ConvertTimeType`](converttimetype.md) | Converts a time data type to another time data type. |
| [`CPUAffinitySet`](cpuaffinityset.md) | Specifies which processors DIAdem uses in a multiprocessor environment. |
| [`CreateEMailService`](createemailservice.md) | Creates an EMailService object . The EMailService object connects to the mail server and provides the mail server with the necessary properties. |
| [`CreateExcelWorkbook`](createexcelworkbook.md) | Creates a new Excel workbook or opens an existing Excel file. Excel does not need to be installed on your computer. |
| [`CreateJsonParser`](createjsonparser.md) | Creates a JsonParser object with methods for reading and writing JSON files in UTF8 format and for converting a JSON object into a Dictionary object or a VBS array , or vice versa. |
| [`CreateMQTT`](createmqtt.md) | Creates a MQTT object . The MQTT object provides the Message Queue Telemetry Transport Protocol in DIAdem. The MQTT protocol is an open message protocol for machine-to-machine (M2M) communication for the transmission of telemetry data between devices. The communication of the individual devices between each other occurs over the MQTT broker. The MQTT broker is not an element of DIAdem. |
| [`CreateTime`](createtime.md) | Creates an object that contains the date and time with a nanoseconds resolution. |
| [`CreateUDI`](createudi.md) | Creates a UDI object with which you can use the script driver . |
| [`CreateValueWithUnit`](createvaluewithunit.md) | Generates a ValueWithUnit object . |
| [`CurveSnippet`](curvesnippet.md) | Creates a curve section you can insert into the text as an expression. |
| [`CustomHelpShow`](customhelpshow.md) | Opens a user-defined help file in the CHM format. |
| [`D3ApprAnsatzOff`](d3appransatzoff.md) | Clears the checkboxes of all the terms for a 3D approximation setup function. |
| [`DataAreaAppend`](dataareaappend.md) | Copies a data block from channels and appends the data block to other channels. |
| [`DataAreaClpCopy`](dataareaclpcopy.md) |  |
| [`DataAreaClpPaste`](dataareaclppaste.md) |  |
| [`DataAreaCopy`](dataareacopy.md) | Copies a data block from channels and inserts the data block into other channels. DIAdem overwrites existing values. |
| [`DataAreaDel`](dataareadel.md) | Deletes a data block in channels. |
| [`DataAreaInsert`](dataareainsert.md) | Copies a data block from channels and inserts the data block into other channels. In the process DIAdem moves existing values down. |
| [`DataAreaInsert0`](dataareainsert0.md) | Inserts a data block with zeros into channels. In the process DIAdem moves existing values down. |
| [`DataAreaInsertV`](dataareainsertv.md) | Inserts a data block with values into channels. In the process DIAdem moves existing values down. |
| [`DataBlAppend`](datablappend.md) | Copies data blocks from channels and appends the data blocks to other channels. |
| [`DataBlClpCopy`](datablclpcopy.md) | Copies a data block from channels into the clipboard. |
| [`DataBlClpPaste`](datablclppaste.md) | Pastes a data block from the clipboard into channels. DIAdem moves existing values down. |
| [`DataBlCopy`](datablcopy.md) | Copies a data block from channels and inserts the data block into other channels. DIAdem overwrites existing values. |
| [`DataBlDel`](databldel.md) | Deletes a data block in channels. |
| [`DataBlInsert`](datablinsert.md) | Copies a data block from channels and inserts the data block into other channels. In the process DIAdem moves existing values down. |
| [`DataBlInsertVal`](datablinsertval.md) | Inserts a data block, in which all the values are the same, into channels. DIAdem moves existing values down. |
| [`DataChangedClear`](datachangedclear.md) | Marks the internal data area as unchanged. The DataChanged variable receives information about whether the internal data area contains modified data. |
| [`DataDBaseLoad`](datadbaseload.md) |  |
| [`DataDelAll`](datadelall.md) |  |
| [`DataDIFLoad`](datadifload.md) |  |
| [`DataERGLoad`](dataergload.md) |  |
| [`DataFileCopy`](datafilecopy.md) | Copies .tdm , .tdms , or .dat type DIAdem files and the associated binary files containing the bulk data. If you save the data file to another target folder, DIAdem does not automatically copy the video files of the video channels, nor does it change the associated relative paths. |
| [`DataFileDelete`](datafiledelete.md) | Deletes .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. If you delete the data file, DIAdem does not automatically delete the video files of the video channels as well. |
| [`DataFileImport`](datafileimport.md) |  |
| [`DataFileLoad`](datafileload.md) | Loads data files into the DIAdem Data Portal. |
| [`DataFileLoadRed`](datafileloadred.md) | Loads data files into the DIAdem Data Portal and simultaneously reduces the data. |
| [`DataFileLoadSel`](datafileloadsel.md) | Loads selected channels from a data file into the DIAdem Data Portal. |
| [`DataFileLstGet`](datafilelstget.md) | Reads a DIAdem file that is a .tdm , .tdms , or .dat type, and creates a list of the associated binary files. The list does not contain video files if the data file contains video channels. |
| [`DataFileMove`](datafilemove.md) | Moves .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. If you save the data file to another target folder, DIAdem does not automatically copy the video files of the video channels, nor does it change the associated relative paths. |
| [`DataFileRename`](datafilerename.md) | Labels .tdm , .tdms , or .dat type DIAdem files and the associated binary files that contain the mass data. |
| [`DataFileSave`](datafilesave.md) | Saves the entire data store from the DIAdem Data Portal, with their properties, to a data file. |
| [`DataFileSaveSel`](datafilesavesel.md) | Saves selected channels and their properties from the DIAdem Data Portal to a data file. DIAdem saves the groups and channels in the target file in the same structure as in the Data Portal. |
| [`DataFileSelDlg`](datafileseldlg.md) | Opens the dialog box for selective loading, in DIAdem NAVIGATOR. |
| [`DataFinderIndexJobFileCreate`](datafinderindexjobfilecreate.md) | Creates a job file for DataFinders. |
| [`DataHISLoad`](datahisload.md) |  |
| [`DataLAXLoad`](datalaxload.md) |  |
| [`DataLoad`](dataload.md) |  |
| [`DataLoadHdFile`](dataloadhdfile.md) | Loads data set properties from a DIAdem Dat data file. |
| [`DataLoadRed`](dataloadred.md) |  |
| [`DataLoadSel`](dataloadsel.md) |  |
| [`DataPreProcessorJobFileCreate`](datapreprocessorjobfilecreate.md) | Creates a job file for the data preparation. |
| [`DataRegistration`](dataregistration.md) |  |
| [`DataSave`](datasave.md) |  |
| [`DataSaveAdd`](datasaveadd.md) | Saves data to an existing DIAdem DAT data file. |
| [`DataSaveSel`](datasavesel.md) |  |
| [`DataSetLoad`](datasetload.md) |  |
| [`DataSetSave`](datasetsave.md) |  |
| [`DDEClose`](ddeclose.md) |  |
| [`DDEExecute`](ddeexecute.md) |  |
| [`DDEGetPokeData`](ddegetpokedata.md) |  |
| [`DDEInit`](ddeinit.md) |  |
| [`DDEOpen`](ddeopen.md) |  |
| [`DDEPokeData`](ddepokedata.md) |  |
| [`DDEPokeText`](ddepoketext.md) |  |
| [`DDERemove`](dderemove.md) |  |
| [`DDERequestData`](dderequestdata.md) |  |
| [`DDERequestText`](dderequesttext.md) |  |
| [`DeskSave`](desksave.md) | Saves the DIAdem desktop file. |
| [`DirListGet`](dirlistget.md) | Generates a list with filenames. |
| [`DirLstWrite`](dirlstwrite.md) | Generates a list with filenames. The command does not support Unicode filenames. Use the DirListGet command instead. |
| [`DlgOpen`](dlgopen.md) | Opens a DIAdem dialog box. |
| [`DocEnd`](docend.md) | Closes the document and sends the print job to the printer. |
| [`DocStart`](docstart.md) | Starts a print job. |
| [`EscapeDatastring`](escapedatastring.md) | Encodes a text using the URL encoding so that the string can be used as a parameter in a URL. With the exception of letters, numbers, and a few special characters, the command replaces each byte of the characters passed with a percent sign and two hexadecimal digits. Do not use this command to encode entire URLs, because the command also encodes the characters "/" and ":". |
| [`ExecuteExclusiveBegin`](executeexclusivebegin.md) | Starts the execution of a script section with mutual exclusion (mutex). Another program instance, which also starts the execution of a mutually exclusive script section for which it uses the same name, will wait for the first instance to finish the execution of the script section. You create a mutual exclusion by inserting the critical script lines into the ExecuteExclusiveBegin and ExecuteExclusiveEnd commands. Use these commands, for example, for parallel processes with multiple Worker objects or within SystemLink TDM to access files exclusively. |
| [`ExecuteExclusiveEnd`](executeexclusiveend.md) | Ends the execution a mutually exclusive script section. If an instance is terminated, the execution of a mutually exclusive script section is automatically released to the other instances. |
| [`ExecuteExclusiveEndAll`](executeexclusiveendall.md) | Ends all executions of mutually exclusive script sections.  If an instance is terminated, the execution of a mutually exclusive script section is automatically released to the other instances. |
| [`ExtProgram`](extprogram.md) | Starts an external program. |
| [`FileAttrClear`](fileattrclear.md) | Deletes file attributes. |
| [`FileAttrSet`](fileattrset.md) | Sets file attributes. |
| [`FileClose`](fileclose.md) | Closes an ASCII file. |
| [`FileCloseAll`](filecloseall.md) | Closes all ASCII files. |
| [`FileCopy`](filecopy.md) | Copies files. |
| [`FileCRCGet`](filecrcget.md) | Specifies the 32 bit long checksum according to the CRC procedure (Cyclic Redundancy Check) for a file. |
| [`FileDateSet`](filedateset.md) | Sets time and date of files. |
| [`FileDelete`](filedelete.md) | Deletes files. |
| [`FileDlgShow`](filedlgshow.md) | Calls the file selection dialog box. |
| [`FileFilterExist`](filefilterexist.md) |  |
| [`FileMove`](filemove.md) | Moves files to another folder. |
| [`FileNameGet`](filenameget.md) | Opens the standard dialog box for loading and saving files. |
| [`FileOpen`](fileopen.md) | Opens ASCII files for reading or writing. |
| [`FileRename`](filerename.md) | Renames files. |
| [`FileWrite`](filewrite.md) | Writes a line without a concluding line break into an ASCII file. |
| [`FileWriteLn`](filewriteln.md) | Possible syntax: FileWriteLn, FW |
| [`FolderAttrClear`](folderattrclear.md) | Deletes folder attributes. |
| [`FolderAttrSet`](folderattrset.md) | Sets folder attributes. |
| [`FolderCopy`](foldercopy.md) | Copies folders and the files they contain to another position. |
| [`FolderCreate`](foldercreate.md) | Creates a folder. |
| [`FolderDelete`](folderdelete.md) | Deletes folders with files. |
| [`FolderDlgShow`](folderdlgshow.md) | Calls the path selection dialog box. |
| [`FolderMove`](foldermove.md) | Moves folders into another folder. |
| [`FolderRename`](folderrename.md) | Renames a folder. |
| [`FolderUnzip`](folderunzip.md) | Unzips a ZIP archive to a folder. |
| [`FolderZip`](folderzip.md) | Compresses a folder to a ZIP archive. |
| [`FontPointsToPixels`](fontpointstopixels.md) | Converts a font size into pixel. DIAdem includes the DPI settings of the system. |
| [`FormulaCalc`](formulacalc.md) | Uses the Calculator AUT syntax to calculate a formula in a script. |
| [`FTP download`](ftp-download.md) | Downloads a file from an FTP server. |
| [`FTPConnect`](ftpconnect.md) | Connects to an FTP server. |
| [`FTPDisConnect`](ftpdisconnect.md) | Disconnects from the FTP server. |
| [`GlobalDim`](globaldim.md) | Declares global variables and reserves memory space for these variables. Global variables are valid and retain their contents as long as DIAdem is running and you do not restart the script engine. |
| [`GlobalReDim`](globalredim.md) | Declares global dynamic array variables and reserves memory space. Global variables are valid and retain their contents as long as DIAdem is running and you do not restart the script engine. |
| [`GPIExtensionRegister`](gpiextensionregister.md) | Registers a GPI extension in DIAdem. It only registers for the running DIAdem instance and is not saved in the desktop file. The registered DLL is not displayed in the GPI Extensions: User Extensions dialog box. |
| [`GPIFileLoad`](gpifileload.md) |  |
| [`GPIFileLoadDlg`](gpifileloaddlg.md) |  |
| [`GPIFileSave`](gpifilesave.md) |  |
| [`GPIFileSaveDlg`](gpifilesavedlg.md) |  |
| [`GPIFileTypeFind`](gpifiletypefind.md) | Specifies the name of a GPI file filter. |
| [`GPSDistance`](gpsdistance.md) | Calculates the shortest distance and the angle from the earth’s center between two coordinates taking the ellipsoidal shape of the Earth into account. |
| [`GraphChangedChk`](graphchangedchk.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphChangedChk command: |
| [`GraphDeleteAll`](graphdeleteall.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphDeleteAll command: |
| [`GraphObjCancel`](graphobjcancel.md) |  |
| [`GraphObjChnClear`](graphobjchnclear.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjChnClear command: |
| [`GraphObjChnNameGet`](graphobjchnnameget.md) |  |
| [`GraphObjClose`](graphobjclose.md) |  |
| [`GraphObjCloseCheck`](graphobjclosecheck.md) |  |
| [`GraphObjDelete`](graphobjdelete.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjDelete command: |
| [`GraphObjDestroy`](graphobjdestroy.md) |  |
| [`GraphObjExist`](graphobjexist.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjExist command: |
| [`GraphObjMove`](graphobjmove.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMove command: |
| [`GraphObjMoveSel`](graphobjmovesel.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveSel command: |
| [`GraphObjMoveToBackground`](graphobjmovetobackground.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveToBackground command: |
| [`GraphObjMoveToForeground`](graphobjmovetoforeground.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjMoveToForeground command: |
| [`GraphObjNew`](graphobjnew.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjNew command: |
| [`GraphObjOpen`](graphobjopen.md) |  |
| [`GraphObjOpenCheck`](graphobjopencheck.md) |  |
| [`GraphObjPositionGet`](graphobjpositionget.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjPositionGet command: |
| [`GraphObjRename`](graphobjrename.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjRename command: |
| [`GraphObjScalingUpdate`](graphobjscalingupdate.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjScalingUpdate command: |
| [`GraphObjSelect`](graphobjselect.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjSelect command: |
| [`GraphObjUnSelectAll`](graphobjunselectall.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjUnSelectAll command: |
| [`GraphObjYAxisNew`](graphobjyaxisnew.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphObjYAxisNew command: |
| [`GraphSheetCopy`](graphsheetcopy.md) |  |
| [`GraphSheetDelete`](graphsheetdelete.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetDelete command: |
| [`GraphSheetInfos`](graphsheetinfos.md) |  |
| [`GraphSheetInsertNew`](graphsheetinsertnew.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetInsertNew command: |
| [`GraphSheetMove`](graphsheetmove.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetMove command: |
| [`GraphSheetNew`](graphsheetnew.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetNew command: |
| [`GraphSheetNGet`](graphsheetnget.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetNGet command: |
| [`GraphSheetRefSet`](graphsheetrefset.md) |  |
| [`GraphSheetRename`](graphsheetrename.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetRename command: |
| [`GraphSheetShow`](graphsheetshow.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSheetShow command: |
| [`GraphSubObjSelect`](graphsubobjselect.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the GraphSubObjSelect command: |
| [`GroupClpCopy`](groupclpcopy.md) | Copies one or more channel groups from the Data Portal to the clipboard. |
| [`GroupClpPaste`](groupclppaste.md) | Pastes one or more channel groups from the clipboard to the Data Portal. |
| [`GroupCopy`](groupcopy.md) |  |
| [`GroupCreate`](groupcreate.md) |  |
| [`GroupDefaultSet`](groupdefaultset.md) |  |
| [`GroupDel`](groupdel.md) |  |
| [`GroupMove`](groupmove.md) |  |
| [`GroupNameChk`](groupnamechk.md) |  |
| [`GroupPropCopy`](grouppropcopy.md) | Copies group properties to another group. You also can use the object-oriented interface to access internal data. Use the AddProperties Properties method to implement the functionality of the GroupPropCopy command with the script interface for internal data. |
| [`GroupPropCreate`](grouppropcreate.md) |  |
| [`GroupPropDel`](grouppropdel.md) |  |
| [`GroupPropExist`](grouppropexist.md) |  |
| [`GroupPropInfoGet`](grouppropinfoget.md) |  |
| [`GroupPropNameChk`](grouppropnamechk.md) |  |
| [`GroupPropSet`](grouppropset.md) |  |
| [`GroupPropValGet`](grouppropvalget.md) |  |
| [`GroupPropValSet`](grouppropvalset.md) |  |
| [`GUIDCreate`](guidcreate.md) | Creates a precise GUID (Globally Unique Identifier) as { XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX }, whereby X is a character from the hexadecimal system, for example, {1BB02FCF-A1A5-4A6E-A3D7-868C429FF05F} . |
| [`HdCopy`](hdcopy.md) | Copies a channel header from one channel to another channel. |
| [`HdCreate`](hdcreate.md) | Generates external channel headers. |
| [`HdDel`](hddel.md) | Deletes an external channel header. |
| [`HdDelAll`](hddelall.md) | Deletes all external channel headers. |
| [`HdLoad`](hdload.md) | Loads the data set properties and channel properties of a data set header file in the DAT format. |
| [`HdMarkAll`](hdmarkall.md) | Marks all channel headers you want to save. |
| [`HdSave`](hdsave.md) | Saves a data set header file in the DAT format. |
| [`HSLtoRGB`](hsltorgb.md) | Converts a color value from the HSL model (Hue, Saturation, Luminosity) into the RGB model (Red, Green, Blue). |
| [`ImageFileAreaToIconFile`](imagefileareatoiconfile.md) | Converts a rectangular extract of a graphic file into an ICO file. |
| [`ImageFileToIconFile`](imagefiletoiconfile.md) | Converts a graphic file into an ICO file. |
| [`InputBoxDisp`](inputboxdisp.md) | Displays one or more prompts in a dialog and returns the contents of the input fields. |
| [`InstallationInfo`](installationinfo.md) | Specifies information about the current installation. |
| [`InteractionOff`](interactionoff.md) | Disables the interaction mode. |
| [`InteractionOn`](interactionon.md) | Enables the interaction mode. |
| [`IsESCKeyPressed`](isesckeypressed.md) | Specifies whether you pressed <Esc> . |
| [`IsKeyPressed`](iskeypressed.md) | Specifies whether the specified key was pressed. |
| [`ItemInfoGet`](iteminfoget.md) | Provides information about a DIAdem variable or a DIAdem command. |
| [`KeyWait`](keywait.md) | Interrupts a script until you press any button. DIAdem displays a message on the status bar. |
| [`LastErrorGet`](lasterrorget.md) |  |
| [`LastErrorReset`](lasterrorreset.md) |  |
| [`LastErrorShow`](lasterrorshow.md) |  |
| [`LastErrorTextGet`](lasterrortextget.md) |  |
| [`LaunchLabVIEW`](launchlabview.md) | Starts the LabVIEW program and opens a VI. |
| [`LevenshteinDist`](levenshteindist.md) | Specifies the Levenshtein distance which is a value for the difference between two texts. |
| [`LogfileBrowser`](logfilebrowser.md) | Opens the current DIAdem logfile in the editor. |
| [`LogfileDel`](logfiledel.md) | Deletes the current logfile in DIAdem. |
| [`LogfileWrite`](logfilewrite.md) | Valid names: LogfileWrite, Print |
| [`LoopDeInit`](loopdeinit.md) | Ends a progress bar display in the status bar. Use the LoopInit command to initialize the progress bar display in the status bar. |
| [`LoopInc`](loopinc.md) | Modifies the percentage of the progress bar in the status bar. For example, if you assign the value 50 to the LoopLength parameter, DIAdem shows only half of the progress bar. Use the LoopInit command to initialize the progress bar and the LoopDeInit command to terminate the progress bar. |
| [`LoopInit`](loopinit.md) | Initializes the progress bar with a percentage in the status bar. Use the LoopInc command to change the value of the progress bar. |
| [`MatAdd`](matadd.md) | Adds two matrices componentwise. |
| [`MatAppend`](matappend.md) | Appends a matrix to a matrix. |
| [`MatChnConvert`](matchnconvert.md) | Converts three-dimensional data matrices, including the x and the y-channel, into a data triplet. |
| [`MatD3Appr`](matd3appr.md) | Uses a setup function to approximate a surface for three-dimensional matrix data. |
| [`MatD3Interp`](matd3interp.md) | Calculates a three-dimensional interpolation for an x-channel, a y-channel, and a z-matrix. |
| [`MatD3InterpPoint`](matd3interppoint.md) | Calculates a single z-value of a three-dimensional interpolation for an x-channel, a y-channel, and a z-matrix. |
| [`MatDiv`](matdiv.md) | Divides two matrices componentwise. |
| [`MatExtremeValues`](matextremevalues.md) | Determines the minimum value and the maximum value of a matrix. |
| [`MatIntegrate`](matintegrate.md) | Calculates the volume under a surface that is specified by a matrix. |
| [`MatIsolinesCalc`](matisolinescalc.md) | Calculates contour lines on a surface with a matrix. |
| [`MatMul`](matmul.md) | Multiplies two matrices. |
| [`MatNormalize`](matnormalize.md) | Normalizes the elements of a matrix to the maximum value one. |
| [`MatRainCalc`](matraincalc.md) | Evaluates a rainflow or transition matrix. |
| [`MatRelativize`](matrelativize.md) | Determines for each element of a matrix the percentage the element has of the total sum of all matrix elements. |
| [`MatScalAdd`](matscaladd.md) | Adds a scalar value componentwise to a matrix. |
| [`MatScalMul`](matscalmul.md) | Multiplies a matrix componentwise by a scalar value. |
| [`MatSort`](matsort.md) | Sorts the values of the x and of the y-channel in a matrix monotonic increasing. DIAdem transposes the z-matrix values according to the new order. |
| [`MatSub`](matsub.md) | Subtracts two matrices componentwise. |
| [`MatSum`](matsum.md) | Calculates the sum of the rows and the sum of the columns in a matrix. |
| [`MatTranspose`](mattranspose.md) | Transposes rows and columns in a matrix. |
| [`MatVAlgebr`](matvalgebr.md) | Multiplies a matrix algebraically by a vector. |
| [`MatVColumn`](matvcolumn.md) | Multiplies a matrix columnwise by a vector. |
| [`MatVRow`](matvrow.md) | Multiplies a matrix rowwise by a vector. |
| [`MenuItemAdd`](menuitemadd.md) |  |
| [`MenuItemChange`](menuitemchange.md) |  |
| [`MenuItemCountGet`](menuitemcountget.md) |  |
| [`MenuItemDel`](menuitemdel.md) |  |
| [`MenuItemInfoGet`](menuiteminfoget.md) |  |
| [`MenuItemInsert`](menuiteminsert.md) |  |
| [`MenuReset`](menureset.md) |  |
| [`MsgBoxCancel`](msgboxcancel.md) | Closes a non-modal message box. |
| [`MsgBoxDisp`](msgboxdisp.md) | Displays a message in a message box. |
| [`MsgBoxSetPos`](msgboxsetpos.md) | Specifies the size and position of the next message box. |
| [`MsgBoxStateResetAll`](msgboxstateresetall.md) | Resets the setting for all dialog boxes so that some dialogs are only displayed when the Shift key is pressed. After executing this command, DIAdem displays the dialog boxes again for which you selected the option Only display this message when the Shift key is pressed . |
| [`MsgButtonTextSet`](msgbuttontextset.md) | Changes the button labels in the next message box. |
| [`MsgLineDisp`](msglinedisp.md) | Displays a message in the status bar. |
| [`OLEChnCommentGet`](olechncommentget.md) |  |
| [`OLEChnCommentGet`](olechncommentget-2.md) |  |
| [`OLEChnDimGet`](olechndimget.md) |  |
| [`OLEChnDimSet`](olechndimset.md) |  |
| [`OLEChnLengthGet`](olechnlengthget.md) |  |
| [`OLEChnLengthSet`](olechnlengthset.md) |  |
| [`OLEChnNameGet`](olechnnameget.md) |  |
| [`OLEChnNameSet`](olechnnameset.md) |  |
| [`OLEChnParaUpdate`](olechnparaupdate.md) |  |
| [`OLEChnValGet`](olechnvalget.md) |  |
| [`OLEChnValSet`](olechnvalset.md) |  |
| [`OLECmdExecute`](olecmdexecute.md) |  |
| [`OLECmdExecuteAsy`](olecmdexecuteasy.md) |  |
| [`OLEDoubleVarGet`](oledoublevarget.md) |  |
| [`OLEDoubleVarSet`](oledoublevarset.md) |  |
| [`OLEIntegerVarGet`](oleintegervarget.md) |  |
| [`OLEIntegerVarSet`](oleintegervarset.md) |  |
| [`OLEInterfaceLock`](oleinterfacelock.md) | Blocks or opens the OLE interfaces TOCommand and TODataSheet . |
| [`OLEMaxChnLenGet`](olemaxchnlenget.md) |  |
| [`OLEMaxChnNoGet`](olemaxchnnoget.md) |  |
| [`OLETextVarGet`](oletextvarget.md) |  |
| [`OLETextVarSet`](oletextvarset.md) |  |
| [`OLEUpdateParaFix`](oleupdateparafix.md) |  |
| [`OLEValueRangeSet`](olevaluerangeset.md) |  |
| [`OpenDocument`](opendocument.md) | Returns an object which provides methods and properties for reading or editing the metadata of a document. |
| [`OrdAFParaSet`](ordafparaset.md) | Sets the parameters for Order analysis in the frequency domain according to the input channels. |
| [`OrdATParaSet`](ordatparaset.md) | Sets the parameters for Order analysis in the time domain according to the input channels. |
| [`PathAddTrailingBackslash`](pathaddtrailingbackslash.md) | Adds a trailing backslash \ to a path. The path then fulfils the DIAdem requirements. If the path already ends with a backslash, DIAdem does not add a second backslash. |
| [`PathDlgShow`](pathdlgshow.md) | Possible spellings: PathDlgShow, PathNameGet, DlgPathSelect |
| [`PathExpand`](pathexpand.md) | Changes a relative path into an absolute path. The input path can contain ".", "..", "/" and "\". The command does not check whether the path exists. |
| [`Pause`](pause.md) | Stops a script for a specific period of time in seconds. DIAdem displays the remaining pause time on the status bar. |
| [`PicDelete`](picdelete.md) |  |
| [`PicExport`](picexport.md) |  |
| [`PicFileAppend`](picfileappend.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicFileAppend command: |
| [`PicHtmlExport`](pichtmlexport.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicHtmlExport command: |
| [`PicLoad`](picload.md) |  |
| [`PicMaxPageCalc`](picmaxpagecalc.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicMaxPageCalc command: |
| [`PicPdfExport`](picpdfexport.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicPdfExport command: |
| [`PicPrint`](picprint.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicPrint command: |
| [`PicPrintDlg`](picprintdlg.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicPrintDlg command: |
| [`PicPrintNoDlg`](picprintnodlg.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the PicPrintNoDlg command: |
| [`PicSave`](picsave.md) |  |
| [`PicSaveAs`](picsaveas.md) |  |
| [`PictureToClipboard`](picturetoclipboard.md) |  |
| [`PicUpdate`](picupdate.md) |  |
| [`PrinterDlg`](printerdlg.md) | Opens the printer dialog box in DIAdem and changes the print settings without printing the current report. |
| [`PrinterPaperSizeGet`](printerpapersizeget.md) | Receives the paper format of the printer. |
| [`PrinterPaperSizeListGet`](printerpapersizelistget.md) | Specifies a list of paper formats that the printer supports. You can use the returned names directly in scripts. |
| [`PrinterPaperSizeSelectable`](printerpapersizeselectable.md) | Specifies whether a paper format can be selected. |
| [`PrinterPaperSizeSet`](printerpapersizeset.md) | Specifies the paper format of the printer. |
| [`PrintMaxScale`](printmaxscale.md) | Specifies the minimum margins for the current printer and the specified page format. Call this command before calling other print commands. |
| [`ProcessMessages`](processmessages.md) | Interrupts the execution of a script and processes the message queue. |
| [`ProgramExit`](programexit.md) | Exits the program. |
| [`PythonEvaluate`](pythonevaluate.md) | Possible notations: PythonEvaluate, PyEval |
| [`RdeEuAnalysis`](rdeeuanalysis.md) | Analyzes the emissions from motor vehicles measured on public transport journeys according to European standards. |
| [`RdeEuExportData`](rdeeuexportdata.md) | Exports the input data of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.1, Tables 1 and 2. The command assumes that the metadata is stored as group properties of the first channel group. |
| [`RdeEuExportReport1`](rdeeuexportreport1.md) | Exports the interim results of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.2.1, Table 3. The command assumes that the metadata is stored as group properties of the first channel group. |
| [`RdeEuExportReport2`](rdeeuexportreport2.md) | Exports the end results of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.2.2, Table 4, 5, 5a, 5b, and 6. The command assumes that the metadata is stored as group properties of the first channel group. |
| [`RdeEuImportData`](rdeeuimportdata.md) | Imports the data for the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.1, Tables 1 and 2. |
| [`RdeEuImportDataProperties`](rdeeuimportdataproperties.md) | Imports the data for the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.1, Table 1. DIAdem stores the metadata as group properties of the first channel group. |
| [`RdeEuImportReport1`](rdeeuimportreport1.md) | Imports the interim results of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.1, Table 3. |
| [`RdeEuImportReport2`](rdeeuimportreport2.md) | Imports the end results of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.1, Table 4, 5, 5a, 5b, and 6. |
| [`RemoveUserCommandFromEvent`](removeusercommandfromevent.md) | Deletes a single user command from a list of user commands which you assigned to an event . |
| [`ReportMasterAdd`](reportmasteradd.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterAdd command: |
| [`ReportMasterDel`](reportmasterdel.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterDel command: |
| [`ReportMasterLoad`](reportmasterload.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterLoad command: |
| [`ReportMasterNew`](reportmasternew.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterNew command: |
| [`ReportMasterSave`](reportmastersave.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterSave command: |
| [`ReportMasterUpd`](reportmasterupd.md) | The following example shows you how to use the object-oriented interface of DIAdem REPORT instead of the ReportMasterUpd command: |
| [`ResultUnitGet`](resultunitget.md) | Returns the symbol of the result unit for an arithmetic operation. |
| [`RGB`](rgb.md) | Specifies the RGB color value. |
| [`RGBtoHSL`](rgbtohsl.md) | Converts a color value from the RGB model (Red, Green, Blue) into the HSL model (Hue, Saturation, Luminosity). |
| [`RootNameChk`](rootnamechk.md) |  |
| [`RootPropCreate`](rootpropcreate.md) |  |
| [`RootPropDel`](rootpropdel.md) |  |
| [`RootPropExist`](rootpropexist.md) |  |
| [`RootPropInfoGet`](rootpropinfoget.md) |  |
| [`RootPropNameChk`](rootpropnamechk.md) |  |
| [`RootPropSet`](rootpropset.md) |  |
| [`RootPropValGet`](rootpropvalget.md) |  |
| [`RootPropValSet`](rootpropvalset.md) |  |
| [`SchemePrintDlg`](schemeprintdlg.md) | Displays a dialog box and prints a DAC graphic. |
| [`ScriptCmdAdd`](scriptcmdadd.md) | Registers a script that contains user commands. Use user commands to add your own commands to DIAdem or to change existing commands. |
| [`ScriptCmdIsLoaded`](scriptcmdisloaded.md) | Checks whether a script file with user commands is already loaded or not. |
| [`ScriptCMDRegister`](scriptcmdregister.md) | Allows CodeCompletion for encrypted user commands. DIAdem takes the information for CodeCompletion from the TLB file. |
| [`ScriptCmdRemove`](scriptcmdremove.md) | Removes a script that contains user commands. You cannot use the commands defined in this script later in DIAdem. DIAdem deletes all variables generated with GlobalDim . |
| [`ScriptCmdReset`](scriptcmdreset.md) | Restarts the script engine. DIAdem re-initializes all global variables and user commands from user command files and resets the variables to the predefined setting. DIAdem deletes all variables generated with GlobalDim . |
| [`ScriptInclude`](scriptinclude.md) | Integrates a script in another script. |
| [`ScriptStart`](scriptstart.md) | Valid names: ScriptStart, VBSStart |
| [`ScriptStatement`](scriptstatement.md) | Executes a VBS statement in an AUT script. |
| [`SHGetFolderPath`](shgetfolderpath.md) | Specifies folders that the operating system supports. |
| [`Signif`](signif.md) | Rounds the value of the first parameter mathematically to the number of significant places specified in the second parameter. |
| [`Sound`](sound.md) | Emits a sound from the PC loudspeakers. |
| [`SPCProcessCapab`](spcprocesscapab.md) | Calculates the mean, the sigma, and the capability indices of a process. |
| [`SQLiteAddExtension`](sqliteaddextension.md) | Loads an SQLite extension library to SQLite. |
| [`SQLiteClose`](sqliteclose.md) | Closes an SQLite database. |
| [`SQLiteOpen`](sqliteopen.md) | Opens an SQLite database file in read and write mode. If the database does not exist, DIAdem creates a new database property. Since only one database can be open at a time, DIAdem first closes an already open database before opening the new database. |
| [`SQLiteQuery`](sqlitequery.md) | Executes an SQLite database query. |
| [`SRTMDownloadGetStatistics`](srtmdownloadgetstatistics.md) | Specifies various statistical values on the SRTM data within the specified latitude-longitude range. The SRTM data contains a high-resolution digital terrain model of the earth surface with the elevation value for nearly every position on the earth. |
| [`SRTMDownloadTilesArea`](srtmdownloadtilesarea.md) | Downloads SRTM data for the specified area into the cache folder. The SRTM data contains a high-resolution digital terrain model of the earth surface with the elevation value for nearly every position on the earth. Use the SRTMDownloadGetStatistics function to get statistical data on the downloaded data. |
| [`StatBlockCalc`](statblockcalc.md) |  |
| [`StatCalc`](statcalc.md) |  |
| [`StopWatchInit`](stopwatchinit.md) | Stops the time measurement and resets the measured value to zero. |
| [`StopWatchPause`](stopwatchpause.md) | Stops the time measurement. |
| [`StopWatchReset`](stopwatchreset.md) | Restarts a time measurement. |
| [`StopWatchStart`](stopwatchstart.md) | Continues the time measurement from the current value. |
| [`StorageImport`](storageimport.md) | Loads data from an external server-based data store into the DIAdem Data Portal. |
| [`SubMat`](submat.md) | Extracts a submatrix from a matrix. |
| [`SubSequence`](subsequence.md) | Identifies a subscript. |
| [`SUDDefLoad`](suddefload.md) | Specifies a SUD file that contains one or more user dialog boxes. |
| [`SUDDlgCreate`](suddlgcreate.md) | Generates a non-modal SUD dialog box. |
| [`SUDDlgCreateEx`](suddlgcreateex.md) | Generates a non-modal SUD dialog box. |
| [`SUDDlgShow`](suddlgshow.md) | Opens a user dialog box. |
| [`SUDEditorStart`](sudeditorstart.md) | Starts the dialog editor. |
| [`SUDNonModalDlgLst`](sudnonmodaldlglst.md) | Receives the list of all non-modal user dialog boxes. |
| [`SysColorGet`](syscolorget.md) | Specifies the current system color of the display element and the control element of an application window. |
| [`TdmsFileDefrag`](tdmsfiledefrag.md) | Defragments a TDMS file in order to read it faster. |
| [`TextClean`](textclean.md) | Removes all characters that cannot be printed, from a string. In the 7-bit ASCII code the characters that cannot be printed are the values 0 to 31 and additionally in the unicode character-set the values 127, 129, 141, 143, 144, and 157. |
| [`TextFileEncoding`](textfileencoding.md) | Specifies the character encoding of a file. The function uses the Byte Order Mark (BOM) of the file to specify the character encoding. |
| [`TextFileEOL`](textfileeol.md) | Specifies the end-of-line character of a text file. The function checks the end-of-line character of the first line. By transferring the end-of-line character to the TextFileOpen function, you can speed up the opening of a text file. |
| [`TextFileOpen`](textfileopen.md) | Opens or creates a text file. |
| [`TextfromClipboard`](textfromclipboard.md) | Returns the contents of the clipboard as text. |
| [`TextToClipboard`](texttoclipboard.md) | Copies a text to the clipboard. |
| [`TTD`](ttd.md) | Converts a text from a time format to a VBS date: A VBS date is a Variant type with the subtype Date . VBS processes data in the range of 01/01/100 to 31/12/9999 23:59:59 . |
| [`UIAutoRefreshSet`](uiautorefreshset.md) | Specifies whether DIAdem informs the Data Portal and the DIAdem VIEW panel about changes to the channel contents or the channel properties while the program is running a script. |
| [`UnEscapeDatastring`](unescapedatastring.md) | Decodes the texts encoded with the EscapeDataString command. |
| [`UserVarCompile`](uservarcompile.md) |  |
| [`UserVarFree`](uservarfree.md) |  |
| [`UserVarFreeAll`](uservarfreeall.md) |  |
| [`UserVarLoad`](uservarload.md) |  |
| [`UserVarReset`](uservarreset.md) |  |
| [`UserVarSave`](uservarsave.md) |  |
| [`ValEqual`](valequal.md) | Checks whether two numeric values are equal. |
| [`ValEqualGT`](valequalgt.md) | Checks whether the first numeric value is greater than or equal to the second numeric value: |
| [`ValEqualLT`](valequallt.md) | Checks whether the first numeric value is less than or equal to the second numeric value: |
| [`ValGT`](valgt.md) | Checks whether the first numeric value is greater than the second numeric value: |
| [`ValLT`](vallt.md) | Checks whether the first numeric value is smaller than the second numeric value: |
| [`ValMax`](valmax.md) | Determines the greater of two numbers. |
| [`ValMin`](valmin.md) | Determines the smaller of two numbers. |
| [`ValueToChn`](valuetochn.md) | Possible spellings: ValueToChn, VariantToChn |
| [`ValueUnitConvert`](valueunitconvert.md) | Converts a numeric value from one unit to a different unit. |
| [`VEnumIdx`](venumidx.md) | Specifies the index of a selection term from an enumeration variable or from a dynamic enumeration variable . |
| [`WeightedReg`](weightedreg.md) | Calculates a linear-weighted regression. |
| [`WinHelpCall`](winhelpcall.md) | Opens a help file with the extension .hlp or .chm. |
| [`WizardStart`](wizardstart.md) | Starts a wizard. |
| [`WndOpen`](wndopen.md) | Opens a DIAdem panel. |
| [`WndShow`](wndshow.md) | Opens or closes a DIAdem panel. |
| [`XOffsetCalc`](xoffsetcalc.md) | Determines the maximum offset of a cross correlation. |
