---
title: "Variables (DAC Block: Alarm)"
---

# Variables

78 variables from `Gfsalarm.chm`.

| Name | Summary |
| --- | --- |
| [`PkAlActive`](pkalactive.md) | Specifies whether the alarm definition that is specified by the index, is activated. |
| [`PkAlAppend`](pkalappend.md) | Specifies whether DIAdem deletes and recreates the logfile at the beginning of a measurement. If you assign the value FALSE to the PkAlAppend variable, DIAdem creates a new logfile. If you assign the value TRUE to the PkAlAppend variable, DIAdem appends new logfile entries to the existing entries. |
| [`PkAlAttachFile`](pkalattachfile.md) | Specifies the name of a file that is to be sent as an attachment. |
| [`PkAlAttachFlag`](pkalattachflag.md) | Specifies whether DIAdem sends a file as an attachment. |
| [`PkAlBackName`](pkalbackname.md) | Specifies the name of the security logfile, including the filename extension. |
| [`PkAlBackup`](pkalbackup.md) | Specifies whether DIAdem creates a security logfile. |
| [`PkAlChn`](pkalchn.md) | Specifies the index of the alarm definition that is to be monitored. |
| [`PkAlChnName`](pkalchnname.md) | Specifies the channel name of the alarm definition that the index references. |
| [`PkAlComment`](pkalcomment.md) | Specifies the comment for an alarm definition. |
| [`PkAlConfirmAll`](pkalconfirmall.md) | Specifies whether DIAdem confirms all the alarms that are selected in the table. If you assign the value 1 to the PkAlConfirmAll variable, DIAdem confirms all the alarms. Otherwise, DIAdem confirms only the selected alarms. |
| [`PkAlDdeFoot`](pkalddefoot.md) | Specifies a trailing text, which DIAdem appends to a text that is to be sent via DDE. |
| [`PkAlDdeHeader`](pkalddeheader.md) | Specifies a leading text, which DIAdem inserts before a text that is to be sent via DDE. |
| [`PkAlDdeItem`](pkalddeitem.md) | Specifies the name of an item for DDE communication. |
| [`PkAlDdeServer`](pkalddeserver.md) | Specifies the name of the DDE server application. |
| [`PkAlDdeTopic`](pkalddetopic.md) | Specifies the name of the topic of the DDE communication. |
| [`PkAlDefCount`](pkaldefcount.md) | Specifies the number of alarm definitions in the alarm generator. If you enter a number that is lower than the number that the alarm generator contains, DIAdem rejects the remaining alarm definitions. |
| [`PkAlDelay`](pkaldelay.md) | Specifies the delay for an alarm definition. |
| [`PkAlFileName`](pkalfilename.md) | Specifies the name of the logfile. |
| [`PkAlFltGroup`](pkalfltgroup.md) | Specifies the names of the alarm groups that are to be displayed. |
| [`PkAlFltGroupCnt`](pkalfltgroupcnt.md) | Specifies the number of alarm groups that are to be displayed. |
| [`PkAlFltPriority`](pkalfltpriority.md) | Specifies the names of the priorities that are to be displayed. |
| [`PkAlFltPtyCnt`](pkalfltptycnt.md) | Specifies the number of priorities that are to be displayed. |
| [`PkAlFltQLCnt`](pkalfltqlcnt.md) | Specifies the number of quit levels that are to be displayed. |
| [`PkAlFltQuitLevel`](pkalfltquitlevel.md) | Specifies the names of the quit levels that are to be displayed. |
| [`PkAlFltState`](pkalfltstate.md) | Specifies the names of the alarm states that are to be displayed. |
| [`PkAlFltStateCnt`](pkalfltstatecnt.md) | Specifies the number of alarm states that are to be displayed. |
| [`PkAlFmtString`](pkalfmtstring.md) | Specifies a format string. |
| [`PkAlFoot`](pkalfoot.md) | Specifies the end text of the logfile. DIAdem writes this end text to the logfile after each measurement. |
| [`PkAlFormat`](pkalformat.md) | Specifies the current format string. |
| [`PkAlFrame`](pkalframe.md) | Specifies whether DIAdem displays a frame. |
| [`PkAlFrameColor`](pkalframecolor.md) | Specifies the color of the frame. |
| [`PkAlGroup`](pkalgroup.md) | Specifies the names of the defined alarm groups. |
| [`PkAlHeader`](pkalheader.md) | Specifies the start text of the logfile. DIAdem writes the start text to the logfile at the beginning of each measurement. |
| [`PKALImportance`](pkalimportance.md) | Specifies the topic of the DDE communication. |
| [`PkAlInstrHeight`](pkalinstrheight.md) | Specifies the height of the instrument in DIAdem VISUAL. |
| [`PkAlInstrPosRel`](pkalinstrposrel.md) | Specifies the alignment of the instrument in DIAdem VISUAL. |
| [`PkAlInstrPosX`](pkalinstrposx.md) | Specifies the x-position of the instrument in DIAdem VISUAL. |
| [`PkAlInstrPosY`](pkalinstrposy.md) | Specifies the y-position of the instrument in DIAdem VISUAL. |
| [`PkAlInstrWidth`](pkalinstrwidth.md) | Specifies the width of the instrument in DIAdem VISUAL. |
| [`PkAlLogSizeMax`](pkallogsizemax.md) | Specifies the size that the logfile has to reach for DIAdem to reset the logfile. If you assign the value 0 to the PkAlLogSizeMax variable, DIAdem does not reset the logfile. |
| [`PkAlLogSizeMin`](pkallogsizemin.md) | Specifies the size of the logfile block that is maintained in the file when DIAdem resets the logfile. |
| [`PkAlMailFoot`](pkalmailfoot.md) | Specifies a concluding text that DIAdem sends as a mail. |
| [`PkAlMailHeader`](pkalmailheader.md) | Specifies a leading text that DIAdem sends as mail. |
| [`PkAlMinimized`](pkalminimized.md) | Specifies whether DIAdem minimizes the window during runtime. |
| [`PkAlName`](pkalname.md) | Specifies the name of the referenced alarm definition. |
| [`PkAlNoDraftOffL`](pkalnodraftoffl.md) | Specifies whether DIAdem deactivates the draft mode offline. |
| [`PkAlNoDraftOnL`](pkalnodraftonl.md) | Specifies whether DIAdem deactivates the draft mode online. |
| [`PkAlOnTop`](pkalontop.md) | Specifies whether DIAdem sets a window mode online, in which the window is always visible. |
| [`PkAlPriority`](pkalpriority.md) | Specifies the names of the priorities of an alarm definition. |
| [`PkAlQuitLevel`](pkalquitlevel.md) | Specifies the name of the quit level for an alarm definition. |
| [`PkAlRecipient`](pkalrecipient.md) | Specifies the name of a DDE server application. |
| [`PkAlRefValue`](pkalrefvalue.md) | Specifies the limit for an alarm definition. |
| [`PkAlRemoteFlag`](pkalremoteflag.md) | Specifies whether DIAdem launches MS Outlook on another computer. |
| [`PkAlRemotePC`](pkalremotepc.md) | Specifies the name of the remote computer. |
| [`PkAlRowMax`](pkalrowmax.md) | Specifies the number of rows at which DIAdem automatically resets the display. |
| [`PkAlRowMin`](pkalrowmin.md) | Specifies the number of rows that DIAdem retains when DIAdem deletes the display. |
| [`PkAlShowButton`](pkalshowbutton.md) | Specifies whether DIAdem displays the OK button in the text window. |
| [`PKALSubject`](pkalsubject.md) | Specifies the name of the topic for DDE communication. |
| [`PKALTabBackColor`](pkaltabbackcolor.md) | Specifies the background color of a row in the alarm table. |
| [`PKALTabCaption`](pkaltabcaption.md) | Specifies the column head of the column referenced in an alarm table. |
| [`PkAlTabColCount`](pkaltabcolcount.md) | Specifies the number of columns in an alarm table. |
| [`PkAlTabConfirm`](pkaltabconfirm.md) | Specifies whether DIAdem displays the button for confirming alarms, while a block diagram is running. This requires the output of the alarm table to be connected to the T input of an alarm generator. |
| [`PKALTabDisp`](pkaltabdisp.md) | Specifies the display mode of the column that is referenced in an alarm table. |
| [`PkAlTabHide`](pkaltabhide.md) | Specifies whether DIAdem hides the alarm table as long as no messages are displayed. |
| [`PkAlTabRHAuto`](pkaltabrhauto.md) | Specifies whether DIAdem specifies the row height in the alarm table automatically or uses the value of the PkAlTabRowHeight variable. |
| [`PkAlTabRowHeight`](pkaltabrowheight.md) | Specifies the row height in the alarm table. |
| [`PkAlTabSelColor`](pkaltabselcolor.md) | Specifies the color of the rows that are selected in the alarm table. |
| [`PkAlTabVar`](pkaltabvar.md) | Specifies the alarm attribute that DIAdem displays in the column that is referenced. |
| [`PKALTabWidth`](pkaltabwidth.md) | Specifies the relative width of the referenced column. |
| [`PkAlTimeAuto`](pkaltimeauto.md) | Specifies whether DIAdem automatically adds a time stamp to an entry. |
| [`PkAlTimeOut`](pkaltimeout.md) | Specifies the time in minutes, after which DIAdem automatically logs off a user. |
| [`PkAlTimeOutFlag`](pkaltimeoutflag.md) | Specifies whether DIAdem automatically logs off a user after a specific period of time. |
| [`PkAlTxtClosed`](pkaltxtclosed.md) | Specifies the label for the OK button if the entry window is closed. |
| [`PkAlTxtColor`](pkaltxtcolor.md) | Specifies the color of the label on the OK button. |
| [`PkAlTxtOpen`](pkaltxtopen.md) | Specifies the label for the OK button. |
| [`PkAlTxtX`](pkaltxtx.md) | Specifies the horizontal label. |
| [`PkAlType`](pkaltype.md) | Specifies the alarm type for the alarm definition that is referenced by the index. |
| [`PkAlUnit`](pkalunit.md) | Specifies the unit of the alarm definition that is referenced by the index. |
