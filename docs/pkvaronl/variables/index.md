---
title: "Variables (Online Package Variables)"
---

# Variables

267 variables from `PkVarOnl.chm`.

| Name | Summary |
| --- | --- |
| [`Pk3DDesign`](pk3ddesign.md) | Specifies in packet processing that DIAdem plots a frame around the voltmeter instruments. |
| [`Pk3DShowN`](pk3dshown.md) | Specifies in the packet processing oscilloscope the number of curves to plot in a waterfall diagram or the number values to be displayed in color in the color/campbell diagram. |
| [`PkAboveMsg`](pkabovemsg.md) | Specifies in packet processing the message text for the status display when the data signal exceeds the top alarm limit. |
| [`PkActiveIn`](pkactivein.md) | Specifies the number of the data input on the packet processing multiplexer if the PkCtrlMode variable has the value 1 . |
| [`PkActiveOut`](pkactiveout.md) | Specifies the number of the data output at the packet processing demultiplexer if the PkControl variable has the value 0 . |
| [`PkAllOn`](pkallon.md) | Selects all statistical characteristic values in the statistics dialog box of packet processing. |
| [`PkAMean`](pkamean.md) | Specifies in packet processing that DIAdem calculates the arithmetic mean as the statistical characteristic value. |
| [`PkAmplitude`](pkamplitude.md) | Specifies in packet processing the amplitude of the generator signal. |
| [`PkAmplType`](pkampltype.md) | Specifies in packet processing which spectrum DIAdem calculates from the results of a FFT. |
| [`PkAmplUnit`](pkamplunit.md) | Specifies in packet processing the amplitude unit of the function generator. |
| [`PkAnalysis`](pkanalysis.md) | Specifies in packet processing whether DIAdem runs a third analysis or an octave analysis. |
| [`PkAppend`](pkappend.md) | Specifies in packet processing that DIAdem appends the data to be written if the data file already exists. The new data must have the same number of channels and the same data format as the file that already exists. |
| [`PkAScaling`](pkascaling.md) | Specifies in packet processing that DIAdem runs an A-scaling for the noise level in decibel [dB] for a third or octave analysis. |
| [`PkAsync`](pkasync.md) | Specifies in packet processing when DIAdem transfers data packets at the active data input of the multiplexer. |
| [`PkAttenuation`](pkattenuation.md) | Specifies in packet processing the attenuation for the elliptic and the inverse Chebyshev filter. |
| [`PkAuto`](pkauto.md) | Specifies in packet processing that DIAdem scales the display area of a display instrument like the incoming data packets. |
| [`PkAutoScalOn`](pkautoscalon.md) | Specifies in packet processing that DIAdem scales the y-axis of the oscilloscope like the incoming data packets. If you assign the value 0 to the PkAutoScalOn variable, DIAdem scales the y-axis according to the specified start value and end value. |
| [`PkAverageSource`](pkaveragesource.md) | Specifies in packet processing whether DIAdem calculates the average of an FFT from the amplitude or from the autospectrum. |
| [`PkAverageType`](pkaveragetype.md) | Specifies in packet processing which mean value DIAdem calculates for an FFT of two time signals. |
| [`PkAvgFactor`](pkavgfactor.md) | Specifies in packet processing to what extent DIAdem uses previous data when calculating the current mean value for the FFT of two time signals. If you assign the value 1 to the PkAvgFactor variable, DIAdem weights all data in a data packet equally. The smaller the weighting factor you select, the less previously calculated data packets are used to calculate the mean value. |
| [`PkBegin`](pkbegin.md) | Specifies in packet processing the bottom limit value of the first class of an online classification. |
| [`PkBelowMsg`](pkbelowmsg.md) | Specifies in packet processing the message text for the status display when the data signal undershoots the bottom alarm limit. |
| [`PkBitCol`](pkbitcol.md) | Specifies in packet processing the number of columns which in turn specifies the arrangement of the switches in a bit switch. |
| [`PkBitNumb`](pkbitnumb.md) | Specifies in packet processing the number of bits for a bit switch. |
| [`PkBlockInc`](pkblockinc.md) | Specifies the number of data packets to be written into a file with the packet processing. DIAdem sets a serial index at the end of the filename or replaces the filename extension with a serial index. |
| [`PkBlockSize`](pkblocksize.md) | Specifies in some packet blocks the packet size of the data packets to be generated or read. |
| [`PkButTxtOff`](pkbuttxtoff.md) | Specifies in packet processing a text for the switched off mode of switches, push buttons, and bit switches. |
| [`PkButTxtOn`](pkbuttxton.md) | Specifies in packet processing a text for the switched on mode of switches, push buttons, and bit switches. |
| [`PkCalcMode`](pkcalcmode.md) | Specifies in packet processing how DIAdem calculates the cumulative frequencies of an online classification. Regardless of the total number of all values, the relative cumulative frequencies of all classes is always 100. DIAdem displays the absolute cumulative frequencies. |
| [`PkChangeSz`](pkchangesz.md) | Specifies in packet processing whether the offset register changes the packet size. Use this variable, for example, to merge data packets that contain only one value per data channel to large data packets, and to output them overlapping. |
| [`PkChNumber`](pkchnumber.md) | Specifies in packet processing the number of a data channel to be read from a file. If you assign the value 0 to the PkChNumber variable, DIAdem reads all data channels of the file. |
| [`PkChS`](pkchs.md) | Specifies in packet processing whether DIAdem writes data into one data channel or into several data channels. DIAdem creates the new data channels in the default group of the Data Portal. |
| [`PkClock`](pkclock.md) | Specifies in packet processing the Sampling rate for reading and transferring single values via the serial interface. |
| [`PkClockRate`](pkclockrate.md) | Specifies the default sampling rate that DIAdem uses for all acquisition blocks in packet processing. |
| [`PkCoherence`](pkcoherence.md) | Specifies in packet processing whether DIAdem calculates the coherence for an FFT of two signals with a joint time channel. |
| [`PkColLimit`](pkcollimit.md) | Specifies in packet processing that the voltmeter highlights in color when the limit values are exceeded or undershot. The voltmeter displays the valid value range in green, the warning range in yellow, and the alarm range in red. |
| [`PkCommApp`](pkcommapp.md) | Specifies in packet processing the text to be appended to a file comment. |
| [`PkCommNew`](pkcommnew.md) | Specifies in packet processing the comment to be saved with the data. |
| [`PkCompany`](pkcompany.md) | Specifies in packet processing the company logo that is to be saved with the written data. |
| [`PkControl`](pkcontrol.md) | Specifies in packet processing the data output number at the demultiplexer for data output. |
| [`PkControl`](pkcontrol-2.md) | Specifies in packet processing whether a control signal, a data signal, or the user controls the transmission and the distribution of data packets to the data outputs of a relay. |
| [`PkCountBlocks`](pkcountblocks.md) | Specifies the period in which the packet processing counter outputs data packets. |
| [`PkCountMode`](pkcountmode.md) | Specifies in packet processing whether the counter counts measurement values, data packets, or time spans. |
| [`PkCrossSpectr`](pkcrossspectr.md) | Specifies in packet processing whether the FFT of two signals calculates the cross spectrum or the transfer function. |
| [`PkCtrlMode`](pkctrlmode.md) | Specifies the data input from which the packet processing multiplexer reads and outputs data. |
| [`PkCursLeft`](pkcursleft.md) | Receives in packet processing the point number of the left cursor in the measurement data window of the oscilloscope. |
| [`PkCursRight`](pkcursright.md) | Receives in packet processing the point number of the right cursor in the measurement data window of the oscilloscope. |
| [`PkCutoffFreq`](pkcutofffreq.md) | Specifies in packet processing the 3 dB-limit frequency for highpass and lowpass digital filters. |
| [`PkDataOnReset`](pkdataonreset.md) | Specifies in packet processing whether DIAdem outputs the mean values of a FFT of two signals only after a reset. Use this variable to control the data flow in order to transfer data packets after a reset. |
| [`PKDataPkLength`](pkdatapklength.md) | Specifies in packet processing the number of values in a data packet. |
| [`PkDecPlaces`](pkdecplaces.md) | Specifies in packet processing the number of decimal places in the numeric display of the voltmeter. |
| [`PkDecPlaces`](pkdecplaces-2.md) | Specifies the number of places after the decimal point, for digital display in packet processing. |
| [`PkDefClock`](pkdefclock.md) | Specifies in packet processing whether the function generator uses the sampling rate and the block size set in Settings»Packet Processing»Default System Clock to generate data packets. |
| [`PkDepartm`](pkdepartm.md) | Specifies in packet processing the department name to be saved with the data. |
| [`PkDispDigi`](pkdispdigi.md) | Specifies in packet processing whether DIAdem shows a numeric display in the voltmeter. |
| [`PkDispPhMax`](pkdispphmax.md) | Specifies in packet processing whether DIAdem identifies the greatest measurement value in the voltmeter, with a marker. |
| [`PkDispPhMin`](pkdispphmin.md) | Specifies in packet processing whether DIAdem identifies the smallest measurement value in the voltmeter, with a marker. |
| [`PkDispScala`](pkdispscala.md) | Specifies in packet processing whether DIAdem displays a scale in the voltmeter. |
| [`PkDispTrend`](pkdisptrend.md) | Specifies in packet processing whether DIAdem displays the measurement data trend in the voltmeter. |
| [`PkDuration`](pkduration.md) | Specifies in packet processing whether DIAdem transfers all data packets or a specific number of data packets after a trigger event. |
| [`PkEnd`](pkend.md) | Specifies in packet processing the top limit value of the last class of an online classification. |
| [`PkFilterLength`](pkfilterlength.md) | Specifies for digital filters in packet processing the number of values to be calculated for FIR filters. |
| [`PkFilterMode`](pkfiltermode.md) | Specifies in packet processing the filter type of digital filters. |
| [`PkFilterOrder`](pkfilterorder.md) | Specifies in packet processing the order of IIR filters. |
| [`PkFilterType`](pkfiltertype.md) | Specifies in packet processing the IIR filter type. |
| [`PkFIRFilter`](pkfirfilter.md) | Specifies in packet processing the digital filter type to be calculated. |
| [`PkFmInput`](pkfminput.md) | Specifies in packet processing how the function generator uses the data of the signal input FM. |
| [`PkFormat`](pkformat.md) | Specifies in packet processing the written File format . |
| [`PkFormelTxt`](pkformeltxt.md) | Specifies in packet processing the formula to be calculated. |
| [`PkFreqOut`](pkfreqout.md) | Specifies in packet processing how fast DIAdem outputs level calculations. |
| [`PkFrequency`](pkfrequency.md) | Specifies in packet processing the limit frequency or the mean frequency of digital filters. |
| [`PkFrequency`](pkfrequency-2.md) | Specifies in packet processing the frequency of a sine signal, a rectangle signal, triangle signal, or an impulse signal generated by a function generator. |
| [`PkFunction`](pkfunction.md) | Specifies in packet processing how DIAdem calculates the data of two packet buses. |
| [`PkFunction`](pkfunction-2.md) | Specifies in packet processing the function of the spectral analysis. |
| [`PkFunction`](pkfunction-3.md) | Specifies in packet processing the IIR filter type for digital filters. |
| [`PkFunction`](pkfunction-4.md) | Specifies in packet processing which window function to use. |
| [`PkFunction`](pkfunction-5.md) | Specifies in packet processing the statistical characteristic values to be calculated for each data packet. |
| [`PkFunction`](pkfunction-6.md) | Specifies in packet processing the mathematical function to be calculated. |
| [`PkGMean`](pkgmean.md) | Specifies in packet processing that DIAdem calculates the geometric mean as the statistical characteristic value. |
| [`PkGreaterOn`](pkgreateron.md) | Specifies in packet processing whether DIAdem monitors when a specific limit value is exceeded. |
| [`PkGreaterVal`](pkgreaterval.md) | Specifies in packet processing the limit value to be exceeded. |
| [`PkHMean`](pkhmean.md) | Specifies in packet processing whether DIAdem calculates the harmonic mean as the statistical characteristic value. |
| [`PkHoldPack`](pkholdpack.md) | Specifies in packet processing whether DIAdem saves data packets at inactive data inputs of the multiplexer to the clipboard and does not reject the data packets. DIAdem always evaluates data packets at the control input. |
| [`PkHyst`](pkhyst.md) | Specifies in packet processing the hysteresis as a percentage of the class width of the online classification. Use the hysteresis to eliminate slight oscillations. |
| [`PkInPacketT`](pkinpackett.md) | Specifies in packet processing that DIAdem saves the data packets that arrive at the replicator during a repetition cycle, to the clipboard. |
| [`PkKaiserWindow`](pkkaiserwindow.md) | Specifies in packet processing whether DIAdem calculates the Kaiser window for FIR filters. |
| [`PkLegendeOn`](pklegendeon.md) | Specifies in packet processing whether DIAdem displays the curve legend in the oscilloscope display window. |
| [`PkLinExtRefTmp`](pklinextreftmp.md) | Specifies in packet processing whether DIAdem uses an offset for thermo linearization. |
| [`PkLinOffsConst`](pklinoffsconst.md) | Specifies in packet processing which temperature value to add for the offset of a thermo linearization. |
| [`PkLinThermoDim`](pklinthermodim.md) | Specifies in packet processing the unit of the physical output value of a thermo linearization. |
| [`PkLinThermoType`](pklinthermotype.md) | Specifies in packet processing the linearization function type of a thermo linearization. You can use DIN EN 60584-1 (IEC 584-1) type thermocouples and a thermolinearization for PT100 type resistance elements. |
| [`PkLowAlrmLmt`](pklowalrmlmt.md) | Specifies in packet processing the bottom alarm limit in the voltmeter. |
| [`PkLowAlrmOn`](pklowalrmon.md) | Specifies in packet processing that DIAdem displays the undershooting of the bottom alarm limit in the voltmeter. |
| [`PkLowerFreq`](pklowerfreq.md) | Specifies in packet processing the lower 3 dB-limit frequency for bandpass or bandstop of digital filters. |
| [`PkLowerLim`](pklowerlim.md) | Specifies in packet processing the bottom window limit of a window trigger. |
| [`PkLowerLimR`](pklowerlimr.md) | Specifies in packet processing the bottom window limit of a retrigger. |
| [`PkLowerOn`](pkloweron.md) | Specifies in packet processing whether DIAdem monitors when a limit value is undershot. |
| [`PkLowerVal`](pklowerval.md) | Specifies in packet processing the limit value of a threshold to be exceeded. |
| [`PkLowWarnLmt`](pklowwarnlmt.md) | Specifies in packet processing the bottom warning limit in the voltmeter. |
| [`PkLowWarnOn`](pklowwarnon.md) | Specifies in packet processing whether DIAdem displays the undershooting of the bottom warning limit in the voltmeter. |
| [`PkMAAVMW`](pkmaavmw.md) | Specifies in packet processing whether DIAdem calculates the average absolute deviation from the mean as a statistical characteristic value. |
| [`PkMax`](pkmax.md) | Specifies in packet processing the end value of the slider control scale and the dial knob. |
| [`PkMaxIndex`](pkmaxindex.md) | Specifies in packet processing the maximum number of files to create when the data is saved. When DIAdem reaches the maximum number of files, DIAdem overwrites the file created first. Use this setting to create a ring buffer. |
| [`PkMergeIn`](pkmergein.md) | Specifies in packet processing the number of signal inputs from which DIAdem collects data packets and merges the data packets to a new multi-channel data packet. |
| [`PkMethod`](pkmethod.md) | Specifies in packet processing the classification method of a classification. |
| [`PkMin`](pkmin.md) | Specifies in packet processing the start value of a slider control scale and a dial scale. |
| [`PkMode`](pkmode.md) | Specifies in packet processing the signal display of the voltmeter. |
| [`PkMode`](pkmode-2.md) | Specifies in packet processing the input instrument for manual input. |
| [`PkMode`](pkmode-3.md) | Specifies in packet processing whether DIAdem determines the classes of an online classification. |
| [`PkMode`](pkmode-4.md) | Specifies in packet processing how DIAdem calculates the arithmetic mean. |
| [`PkMode`](pkmode-5.md) | Specifies in packet processing how DIAdem extracts data from incoming data packets. |
| [`PkMode`](pkmode-6.md) | Specifies in packet processing when the timer outputs a control signal. |
| [`PkName`](pkname.md) | Specifies in packet processing the name and path of the data file to be read or written. |
| [`PkNBlock`](pknblock.md) | Specifies in packet processing the number of repetitions to copy data packets and to output the data packets repeatedly. |
| [`PkNBlock`](pknblock-2.md) | Specifies in packet processing the number of data packets after which DIAdem rejects the current values of an online classification and starts a new count. |
| [`PkNoEditOn`](pknoediton.md) | Specifies in packet processing whether you can operate specific functions in the display window in the oscilloscope. |
| [`PkNormalMsg`](pknormalmsg.md) | Specifies in packet processing the message text for the status display when the data signal is in the valid value range of the voltmeter. |
| [`PkNormMode`](pknormmode.md) | Specifies in packet processing the curve display in the oscilloscope. |
| [`PkNOut`](pknout.md) | Specifies in packet processing the number of signal outputs of a copy. |
| [`PkNPck`](pknpck.md) | Specifies in packet processing the number of data packets to write into the Data Portal. |
| [`PkNumber`](pknumber.md) | Specifies in packet processing the number of classes of an online classification. |
| [`PkNumChanOut`](pknumchanout.md) | Specifies in packet processing the number of signal outputs to output multi-channel data packets as one-channel data packets. |
| [`PkNVal`](pknval.md) | Specifies in packet processing the number of values to write into the Data Portal. |
| [`PkNValues`](pknvalues.md) | Specifies in packet processing the maximum number of values collected in the buffer. |
| [`PkOffset`](pkoffset.md) | Specifies in packet processing the smallest value of the voltmeter display area. |
| [`PkOffsetInMd`](pkoffsetinmd.md) | Specifies in packet processing the offset size in order to output large data packets in smaller overlapping sub-packets with the slider control. |
| [`PkOneBmp`](pkonebmp.md) | Specifies in packet processing whether DIAdem displays a bitmap on all switches of a bit switch. If you assign the value 0 to the variable, DIAdem distributes the loaded bitmap to the switches. |
| [`PkOrder`](pkorder.md) | Specifies in packet processing the filter order of digital filters. High filter orders provide a steeper filter with greater phase displacement |
| [`PkOut`](pkout.md) | Specifies in packet processing the output string to transfer data over a serial interface to an external device. |
| [`PkOutMode`](pkoutmode.md) | Specifiesbin packet processing whether DIAdem outputs the calculated mean values only after a reset. |
| [`PkOutMode`](pkoutmode-2.md) | Specifies in packet processing whether the threshold value outputs a TTL signal or a data signal when the incoming data packets exceed or undershoot limit values. |
| [`PkOutMode`](pkoutmode-3.md) | Specifies in packet processing whether DIAdem outputs all statistical characteristic values in one multi-channel data packet to one data output or in several one-channel data packets to various data outputs in the block diagram. |
| [`PkPackToSend`](pkpacktosend.md) | Specifies in packet processing the number of output data packets to be output after a trigger event. |
| [`PkParam`](pkparam.md) | Specifies in packet processing the type of data amount to be created in sections. |
| [`PkPckOffset`](pkpckoffset.md) | Specifies in packet processing the overlapping width with which the offset register outputs data packets. |
| [`PkPckSz`](pkpcksz.md) | Specifies in packet processing the number of values of a data packet. |
| [`PkPeriod`](pkperiod.md) | Specifies in hours, minutes, and seconds how long the timer of the packet processing outputs a control signal. At the end of the run-time the control signal falls to TTL low. |
| [`PkPermXFrom`](pkpermxfrom.md) | Specifies in packet processing the start value of the x-axis in seconds in order to scale the x-axis of the oscilloscope. |
| [`PkPermXOn`](pkpermxon.md) | Specifies in packet processing a fixed scaling for the x-axis of the oscilloscope. The permanent scaling of the x-axis is possible only for y/x-diagrams. |
| [`PkPermXTo`](pkpermxto.md) | Specifies in packet processing the end value of the x-axis in seconds in order to scale the x-axis of the oscilloscope. |
| [`PkPermYFrom`](pkpermyfrom.md) | Specifies in packet processing the start value of the y-axis in seconds in order to scale the y-axis of the oscilloscope. |
| [`PkPermYOn`](pkpermyon.md) | Specifies in packet processing a fixed scaling for the y-axis of the oscilloscope. |
| [`PkPermYTo`](pkpermyto.md) | Specifies in packet processing the end value of the y-axis in order to scale the y-axis of the oscilloscope. |
| [`PkPhase`](pkphase.md) | Specifies in packet processing the phase of a sine signal, a square signal, triangle signal, and an impulse signal generated by a function generator. |
| [`PkPhaseFFT`](pkphasefft.md) | Specifies in packet processing whether DIAdem calculates the phase spectrum for the FFT. For phase calculation, DIAdem calculates the angle measured counterclockwise between the positive real axis and the appropriate place vector (real part, imaginary part). |
| [`PkPortNr`](pkportnr.md) | Specifies in packet processing the serial interface to which an external device is connected. |
| [`PkPreTrigRange`](pkpretrigrange.md) | Specifies in packet processing how many values DIAdem outputs before a trigger event. The pretrigger range must not exceed the block size. |
| [`PkQFactor`](pkqfactor.md) | Specifies in packet processing the quality factor for bandpass and bandstop of digital filters. |
| [`PkQMean`](pkqmean.md) | Specifies in packet processing whether DIAdem calculates the square mean or the root mean square as the statistical value. |
| [`PkQSum`](pkqsum.md) | Specifies in packet processing whether DIAdem calculates the sum of the squared values of a data packet as a statistical characteristic value. |
| [`PkQuantA`](pkquanta.md) | Specifies in packet processing the number of values or data packets of the first data amount A, to be created in sections. |
| [`PkQuantB`](pkquantb.md) | Specifies in packet processing the number of values or data packets of the second data amount B to be created in sections. |
| [`PkRadio`](pkradio.md) | Specifies in packet processing whether the switches of a multi-channel input instrument switch off each other. |
| [`PkRange`](pkrange.md) | Specifies in packet processing the width of all classes of an online classification. |
| [`PkRange`](pkrange-2.md) | Specifies in packet processing the entire display area of a voltmeter. |
| [`PkRate`](pkrate.md) | Specifies in packet processing the sampling rate of the signal the function generator creates. |
| [`PkRealTime`](pkrealtime.md) | Specifies in packet processing whether the function generator generates data packets as fast as possible or with the specified clock rate and packet size. |
| [`PkRecLength`](pkreclength.md) | Specifies in packet processing the number of values to be displayed simultaneously in the oscilloscope and thereby the display area of the recorder. |
| [`PkReduceVal`](pkreduceval.md) | Specifies in packet processing the number of values in an interval, for which DIAdem calculates the mean value. |
| [`PkRefLine`](pkrefline.md) | Specifies in packet processing the zero line for the classification method, to separate oscillations into positive and negative sections. |
| [`PkRegionType`](pkregiontype.md) | Specifies in packet processing whether the trigger event occurs inside or outside the monitored area. |
| [`PkRepeatM`](pkrepeatm.md) | Specifies in packet processing which data DIAdem reads and how often DIAdem reads the data and outputs the data to the block diagram. |
| [`PkRepeatM`](pkrepeatm-2.md) | Specifies in packet processing how often the replicator repeatedly outputs a data packet to the block diagram. |
| [`PkRepeatM`](pkrepeatm-3.md) | Specifies in packet processing that DIAdem writes a specified number of data packets into the Data Portal. |
| [`PkRepeatMode`](pkrepeatmode.md) | Specifies in packet processing which data DIAdem reads repeatedly from a file. |
| [`PkRepMode`](pkrepmode.md) | Specifies in packet processing that DIAdem reads the data repeatedly and outputs the data to the block diagram. |
| [`PkReset`](pkreset.md) | Specifies in packet processing when DIAdem triggers the reset of an online classification to reject values and to begin a new count. |
| [`PkResetCount`](pkresetcount.md) | Specifies in packet processing the number of data packets after which DIAdem rejects the current values of an FFT and restarts averaging. |
| [`PkResetMode`](pkresetmode.md) | Specifies in packet processing whether DIAdem rejects the current values of an FFT of two time signals or of mean value calculation and restarts averaging. |
| [`PkResNBlocks`](pkresnblocks.md) | Specifies in packet processing the number of data packets after which DIAdem starts a new mean value calculation. |
| [`PkRetrigger`](pkretrigger.md) | Specifies in packet processing whether DIAdem checks a trigger signal continuously for trigger events. |
| [`PkRetrigType`](pkretrigtype.md) | Specifies in packet processing which condition a retrigger activates for the trigger searcher. |
| [`PkRipple`](pkripple.md) | Specifies in packet processing the ripples of digital filters in the pass-band of the Chebyshev and the elliptic filters. |
| [`PkRMS`](pkrms.md) | Specifies in packet processing whether a level calculation calculates the root mean square or the peak of the acoustic pressure. |
| [`PkScale1FactorV`](pkscale1factorv.md) | Specifies in packet processing the factor of a linear scale. |
| [`PkScale1OffsV`](pkscale1offsv.md) | Specifies in packet processing the offset of a linear scale. |
| [`PkScale2Inp1V`](pkscale2inp1v.md) | Specifies in packet processing the scaled measurement value for the first linear point of a two-point-scaling. |
| [`PkScale2Inp2V`](pkscale2inp2v.md) | Specifies in packet processing the scaled value for the second linear point of a two-point-scaling. |
| [`PkScale2Phys1V`](pkscale2phys1v.md) | Specifies in packet processing the measurement value for the first linear point of a 2-point scaling. |
| [`PkScale2Phys2V`](pkscale2phys2v.md) | Specifies in packet processing the measurement value for the second linear point of a 2-point scaling. |
| [`PkScaleDim`](pkscaledim.md) | Specifies in packet processing the unit of the physical output value of a multiple point scaling. |
| [`PkScaleDimV`](pkscaledimv.md) | Specifies in packet processing the unit of the physical output value of a two-point-scaling. |
| [`PkScaleDimV`](pkscaledimv-2.md) | Specifies in packet processing the unit of the physical output value of a linear scale. |
| [`PkScalMax`](pkscalmax.md) | Specifies in packet processing whether DIAdem scales the results of a spectral analysis to a minimum. |
| [`PkScalVal`](pkscalval.md) | Specifies in packet processing the reference point to scale the results of a spectral analysis. |
| [`PkSelChan`](pkselchan.md) | Specifies in packet processing the channel number of the data channel to be checked if the data packets are multi-channel packets. |
| [`PkSizeMax`](pksizemax.md) | Specifies for the section creation in packet processing the maximum number of values that DIAdem collects and outputs through a control signal, in a data packet. DIAdem does not create data packets with a large packet size. |
| [`PkSizeMin`](pksizemin.md) | Specifies when sections are created in packet processing the minimum number of values that DIAdem needs to create a data packet when a control signal manages the control. DIAdem does not create data packets with smaller packet sizes. |
| [`PkSkipVal`](pkskipval.md) | Specifies in packet processing the number of values that DIAdem rejects at the start of a measurement, when creating sections. |
| [`PkSlopeType`](pkslopetype.md) | Specifies in packet processing the type of slope condition to be activated. |
| [`PkSlopeTypeR`](pkslopetyper.md) | Specifies in packet processing the type of retrigger slope condition to be activated. |
| [`PkSmoothNVal`](pksmoothnval.md) | Specifies in packet processing the number of values for calculating the moving average. |
| [`PkSpannw`](pkspannw.md) | Specifies in packet processing whether DIAdem calculates the range from the difference between the highest and the lowest measurement value as a statistical characteristic value. |
| [`PkStart`](pkstart.md) | Specifies in hours, minutes, and seconds when the timer sets the control signal in packet processing to TTL high . Use the syntax hh:mm:ss . |
| [`PkStdAbw`](pkstdabw.md) | Specifies in packet processing whether DIAdem calculates the standard deviation as the statistical characteristic value. |
| [`PkStop`](pkstop.md) | Specifies in packet processing the stop string to deinitialize an external device over the serial interface. |
| [`PkStopAll`](pkstopall.md) | Specifies in packet processing whether DIAdem also stops the single point blocks of a block diagram, which stops the entire measurement. If you assign the variable the value 0 , the single point processing blocks continue after the packet blocks stop. |
| [`PkStopNBlocks`](pkstopnblocks.md) | Specifies after how many data packets DIAdem stops the packet processing. |
| [`PkSumAll`](pksumall.md) | Specifies in packet processing whether DIAdem calculates the sum of all values that have arrived since the start of the measurement. |
| [`PkSumBlock`](pksumblock.md) | Specifies in packet processing whether DIAdem calculates the sum of the measured values in one data packet. |
| [`PkSwitch`](pkswitch.md) | Specifies in packet processing how the relay switch works. |
| [`PkTarget`](pktarget.md) | Specifies in packet processing that DIAdem prints out the protocol lists. |
| [`PkThreshold`](pkthreshold.md) | Specifies in packet processing the threshold value of a slope condition. |
| [`PkThresholdR`](pkthresholdr.md) | Specifies in packet processing the threshold value of the retrigger slope. |
| [`PkTimeHold`](pktimehold.md) | Specifies in packet processing the time in seconds that DIAdem deletes from the level calculation before a pause. |
| [`PkTimeTc`](pktimetc.md) | Specifies in packet processing the time constant for calculating the root mean square of a level calculation. |
| [`PkTimeTx`](pktimetx.md) | Specifies in packet processing a fixed time span in seconds in which DIAdem acquires the maximum level of the clock during a level calculation. |
| [`PkTitle`](pktitle.md) | Specifies in packet processing the title to be saved with the data. |
| [`PkTitleTxt`](pktitletxt.md) | Specifies in packet processing the text that DIAdem shows above the voltmeter display. |
| [`PkTitleTxt`](pktitletxt-2.md) | Specifies in packet processing the text for the label of the input instrument. |
| [`PkTransFctType`](pktransfcttype.md) | Specifies in packet processing the calculation mode of the transfer function for the FFT of two time signals. |
| [`PkTransPhase`](pktransphase.md) | Specifies in packet processing whether DIAdem calculates the phase spectrum for an FFT of two time signals. |
| [`PkTriggMode`](pktriggmode.md) | Specifies in packet processing the triggering of the threshold value. |
| [`PkTrigSignal`](pktrigsignal.md) | Specifies in packet processing which input signal at the trigger block checks DIAdem for trigger events. |
| [`PkTrigType`](pktrigtype.md) | Specifies in packet processing which condition activates a control signal for the trigger search. |
| [`PKType`](pktype.md) | Specifies in packet processing the filter type of digital filters. |
| [`PkUnit`](pkunit.md) | Specifies in packet processing the unit of the data generated manually. |
| [`PkUpAlrmLmt`](pkupalrmlmt.md) | Specifies in packet processing the top alarm limit in the voltmeter. |
| [`PkUpAlrmOn`](pkupalrmon.md) | Specifies in packet processing whether DIAdem displays the exceeding of the top alarm limit in the voltmeter. |
| [`PkUpdateCP`](pkupdatecp.md) | Specifies in packet processing whether DIAdem reads new calibration curves for multiple point scaling, during a measurement. |
| [`PkUpperFreq`](pkupperfreq.md) | Specifies in packet processing the upper 3 dB-limit frequency for bandpass or bandstop of digital filters. |
| [`PkUpperLim`](pkupperlim.md) | Specifies in packet processing the top window limit of a window trigger. |
| [`PkUpperLimR`](pkupperlimr.md) | Specifies in packet processing the top window limit of a retrigger. |
| [`PkUpWarnLmt`](pkupwarnlmt.md) | Specifies in packet processing the top warning limit in the voltmeter. |
| [`PkUpWarnOn`](pkupwarnon.md) | Specifies in packet processing whether DIAdem displays the exceeding of the top warning limit in the voltmeter. |
| [`PkUser`](pkuser.md) | Specifies in packet processing the name of the author to be saved with the data. |
| [`PkUserUnitL`](pkuserunitl.md) | Specifies in packet processing the name of a user unit. |
| [`PkUserUnitS`](pkuserunits.md) | Specifies in packet processing the short form of a user unit. |
| [`PkValue`](pkvalue.md) | Returns in packet processing the current value of an input instrument. |
| [`PkVarianz`](pkvarianz.md) | Specifies in packet processing that DIAdem calculates the variance as the statistical characteristic value. |
| [`PkVarKoeff`](pkvarkoeff.md) | Specifies in packet processing whether DIAdem calculates the variation coefficient as the statistical value. |
| [`PkVarKoRel`](pkvarkorel.md) | Specifies in packet processing whether DIAdem calculates the variation coefficient as statistical characteristic value in percent. |
| [`PkViewMode`](pkviewmode.md) | Specifies in packet processing the signal display of the oscilloscope. |
| [`PkWaveForm`](pkwaveform.md) | Specifies in packet processing the signal form of the signal to be generated. |
| [`PkWFactor`](pkwfactor.md) | Specifies in packet processing to what extent DIAdem uses data of previous data packets to calculate the mean value. If you assign the value 1 to the PkWFactor variable, DIAdem weights all data in a data packet equally. The smaller the weighting factor you select, the less previously calculated data packets are used to calculate the mean value. |
| [`PkWidth`](pkwidth.md) | Specifies in packet processing the class width of an online classification. |
| [`PkWindowFunction`](pkwindowfunction.md) | Specifies in packet processing the windows function of IIR filters. |
| [`PkWindowType`](pkwindowtype.md) | Specifies in packet processing the type of activating windows condition. |
| [`PkWindowTypeR`](pkwindowtyper.md) | Specifies in packet processing the type of activating window condition of a retrigger. |
| [`PkWndCorrectTyp`](pkwndcorrecttyp.md) | Specifies in packet processing the correction of an FFT amplitude attenuation that is caused by the window function. |
| [`PkWndFct`](pkwndfct.md) | Specifies in packet processing the windows function for an FFT. To reduce the spectral broadening, DIAdem multiplies the time signal by the selected window function. |
| [`PkWndPara`](pkwndpara.md) | Specifies in packet processing the parameters for the window functions Kaiser-Bessel, Cauchy, Gauss, and Exponential. |
| [`PkXCh`](pkxch.md) | Specifies in packet processing whether DIAdem creates an x-data channel to every y-data channel when DIAdem writes data. |
| [`PkXCh`](pkxch-2.md) | Specifies in packet processing the sampling rate DIAdem uses to generate an x-channel when reading data. |
| [`PkXMax`](pkxmax.md) | Specifies in packet processing whether DIAdem calculates the greatest time value as the statistical characteristic value. |
| [`PkXMess1`](pkxmess1.md) | Specifies in packet processing the measurement value for the first x-point of a characteristic curve. |
| [`PkXMess2`](pkxmess2.md) | Specifies in packet processing the measurement value for the second x-point of a characteristic curve. |
| [`PkXMin`](pkxmin.md) | Specifies in packet processing whether DIAdem calculates the smallest time value as the statistical characteristic value. |
| [`PkXonYMax`](pkxonymax.md) | Specifies in packet processing whether DIAdem calculates the time value of the maximum measurement value as the statistical characteristic value. |
| [`PkXonYMin`](pkxonymin.md) | Specifies in packet processing whether DIAdem calculates the time value of the minimum measurement value as the statistical characteristic value. |
| [`PkXRate`](pkxrate.md) | Specifies in packet processing the sampling rate for generating the x-channel when DIAdem reads data. |
| [`PkXScal1`](pkxscal1.md) | Specifies in packet processing the scaled measurement value for the first x-point of a characteristic curve. |
| [`PkXScal2`](pkxscal2.md) | Specifies in packet processing the scaled measurement value for the second x-point of a characteristic curve. |
| [`PkXUnit`](pkxunit.md) | Specifies in packet processing the unit for the time axis of a characteristic curve. |
| [`PkXValueMode`](pkxvaluemode.md) | Specifies in packet processing the format of an x-channel to be generated. |
| [`PkXWeight`](pkxweight.md) | Specifies in packet processing that DIAdem evaluates time related and frequency related data such as the results of an FFT or a third analysis with a digital filter order in accordance with DIN IEC 651. |
| [`PkYMax`](pkymax.md) | Specifies in packet processing whether DIAdem calculates the greatest measurement value as the statistical characteristic value. |
| [`PkYMax`](pkymax-2.md) | Specifies for scaling in packet processing the expected top limit for the value range of an input signal. |
| [`PkYMess1`](pkymess1.md) | Specifies in packet processing the measurement value for the first y-point of a characteristic curve. |
| [`PkYMess2`](pkymess2.md) | Specifies in packet processing the measurement value for the second y-point of a characteristic curve. |
| [`PkYMin`](pkymin.md) | Specifies in packet processing whether DIAdem calculates the smallest measurement value as the statistical characteristic value. |
| [`PkYMin`](pkymin-2.md) | Specifies for scaling in packet processing the expected bottom limit for the value range of an input signal. |
| [`PkYonXMax`](pkyonxmax.md) | Specifies in packet processing whether DIAdem calculates the measurement value of the greatest time value as the statistical characteristic value. |
| [`PkYonXMin`](pkyonxmin.md) | Specifies in packet processing whether DIAdem calculates the measurement value of the smallest time value as the statistical characteristic value. |
| [`PkYScal1`](pkyscal1.md) | Specifies in packet processing the scaled measurement value for the first y-point of a characteristic curve. |
| [`PkYScal2`](pkyscal2.md) | Specifies in packet processing the scaled measurement value for the second y-point of a characteristic curve. |
| [`PkYUnit`](pkyunit.md) | Specifies in packet processing the unit for the measurement values of a characteristic curve. |
