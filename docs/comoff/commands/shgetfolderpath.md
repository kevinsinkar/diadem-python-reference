---
title: "SHGetFolderPath"
description: "Specifies folders that the operating system supports."
---

# SHGetFolderPath

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SHGetFolderPath

Specifies folders that the operating system supports.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SHGetFolderCSIDL</td>
<td>Specifies the folders that DIAdem determines with the <a href="./">SHGetFolderPath</a> function.<div id="exp_SHGetFolderCSIDL">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-2147483648 &lt;= SHGetFolderCSIDL &lt;= 2147483647</td></tr>
</table>
<table class="Borderless">
<tr>
<td width="150"><strong>Value</strong></td>
<td><strong>Explanation</strong></td>
</tr>
<tr>
<td width="150">&amp;H0030</td>
<td>Specifies the folder that is used to store administrative tools for an individual user. The Microsoft Management Console (MMC) saves customized consoles to this folder.</td>
</tr>
<tr>
<td width="150">&amp;H001d</td>
<td>Specifies the folder that corresponds to the Startup program group.</td>
</tr>
<tr>
<td width="150">&amp;H001a</td>
<td>Specifies the folder that contains general user defined files. A typical path is <span class="Monospace">C:\Documents and Settings\User\Application Data</span>.</td>
</tr>
<tr>
<td width="150">&amp;H000a</td>
<td>Specifies the virtual folder that contains the recycle bin.</td>
</tr>
<tr>
<td width="150">&amp;H003b</td>
<td>Specifies the folder that contains the data to be written to CD. A typical path is <span class="Monospace">C:\Documents and Settings\username\Application Data\Microsoft\CD Burning</span>.</td>
</tr>
<tr>
<td width="150">&amp;H002f</td>
<td>Specifies the folder that contains the administrative tools for all the users of the computer.</td>
</tr>
<tr>
<td width="150">&amp;H001e</td>
<td>Specifies the folder that corresponds to the Startup program group for all users. Valid only for Windows NT systems.</td>
</tr>
<tr>
<td width="150">&amp;H0023</td>
<td>Specifies the folder that contains general user defined files for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Application Data</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0019</td>
<td>Specifies the folder that contains the desktop files for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Desktop</span>.</td>
</tr>
<tr>
<td width="150">&amp;H002e</td>
<td>Specifies the folder that contains shared files of all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Documents</span>. Valid for Windows NT, Windows 95, and Windows 98 with an installed <span class="Monospace">Shfolder.dll</span>.</td>
</tr>
<tr>
<td width="150">&amp;H001f</td>
<td>Specifies the folder that contains favorites shared by all users. Valid only for Windows NT systems.</td>
</tr>
<tr>
<td width="150">&amp;H0035</td>
<td>Specifies the folder that contains shared music files for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\My Music</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0036</td>
<td>Specifies the folder that contains shared image files for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\My Pictures</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0017</td>
<td>Specifies the folder that contains subfolders for common program groups which appear in the start menu for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Documents\Start Menu\Programs</span>. Valid only for Windows NT systems.</td>
</tr>
<tr>
<td width="150">&amp;H0016</td>
<td>Specifies the folder that contains the shared programs and folders which appear in the start menu for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Documents\Start Menu</span>. Valid only for Windows NT systems.</td>
</tr>
<tr>
<td width="150">&amp;H0018</td>
<td>Specifies the folder that contains the shared programs which appear in the Startup group for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Documents\Startup</span>. Valid only for Windows NT systems.</td>
</tr>
<tr>
<td width="150">&amp;H002d</td>
<td>Specifies the folder that contains templates for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\Templates</span>. Valid only for Windows NT systems.</td>
</tr>
<tr>
<td width="150">&amp;H0037</td>
<td>Specifies the folder that contains shared video files for all users. A typical path is <span class="Monospace">C:\Documents and Settings\All Users\My Videos</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0003</td>
<td>Specifies the virtual folder that contains the symbols for the control panel.</td>
</tr>
<tr>
<td width="150">&amp;H0021</td>
<td>Specifies the folder that contains Internet cookies. A typical path is <span class="Monospace">C:\Documents and Settings\username\Cookies</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0000</td>
<td>Specifies the virtual folder that corresponds to the Windows desktop and to the root of the Explorer.</td>
</tr>
<tr>
<td width="150">&amp;H0010</td>
<td>Specifies the folder that contains the objects of the Windows desktop. A typical path is <span class="Monospace">C:\Documents and Settings\username\Desktop</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0011</td>
<td>Specifies the virtual folder that represents the computer. The folder contains local hard disks, printers, and the control panel. The folder might also contain network drives.</td>
</tr>
<tr>
<td width="150">&amp;H0006</td>
<td>Specifies the folder that contains favorites. A typical path is <span class="Monospace">C:\Documents and Settings\username\Favorites</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0014</td>
<td>Specifies the virtual folder that contains the fonts. A typical path is <span class="Monospace">C:\Windows\Fonts</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0022</td>
<td>Specifies the folder that contains the Internet history items.</td>
</tr>
<tr>
<td width="150">&amp;H0001</td>
<td>Specifies the virtual folder that represents the Internet.</td>
</tr>
<tr>
<td width="150">&amp;H0020</td>
<td>Specifies the folder that contains temporary Internet files. A typical path is <span class="Monospace">C:\Documents and Settings\username\Local Settings\Temporary Internet Files</span>.</td>
</tr>
<tr>
<td width="150">&amp;H001c</td>
<td>Specifies the folder that contains a data collection for local programs. A typical path is <span class="Monospace">C:\Documents and Settings\username\Local Settings\Application Data</span>.</td>
</tr>
<tr>
<td width="150">&amp;H000d</td>
<td>Specifies the folder that contains music files. A typical path is <span class="Monospace">C:\Documents and Settings\username\Documents\My Music</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0027</td>
<td>Specifies the folder that contains picture files. A typical path is <span class="Monospace">C:\Documents and Settings\username\Documents\My Pictures</span>.</td>
</tr>
<tr>
<td width="150">&amp;H000e</td>
<td>Specifies the folder that contains video files. A typical path is <span class="Monospace">C:\Documents and Settings\username\Documents\My Videos</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0013</td>
<td>Specifies the virtual folder that contains possible links to objects in the network neighborhood. A typical path is <span class="Monospace">C:\Documents and Settings\username\Documents\NetHood</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0012</td>
<td>Specifies the virtual folder that represents the root of the network neighborhood.</td>
</tr>
<tr>
<td width="150">&amp;H0005</td>
<td>Specifies the folder that stores documents. A typical path is <span class="Monospace">C:\Documents and Settings\username\My Documents</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0004</td>
<td>Specifies the virtual folder that contains the installed printers.</td>
</tr>
<tr>
<td width="150">&amp;H001b</td>
<td>Specifies the virtual folder that contains the link objects that might exist in the virtual printer folder. A typical path is <span class="Monospace">C:\Documents and Settings\username\Documents\PrintHood</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0028</td>
<td>Specifies the folder of the user profile. A typical path is <span class="Monospace">C:\Documents and Settings\username</span>.</td>
</tr>
<tr>
<td width="150">&amp;H003e</td>
<td>Specifies the folder that contains user profiles. A typical path is <span class="Monospace">C:\Documents and Settings</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0026</td>
<td>Specifies the program folder. A typical path is <span class="Monospace">C:\Program files</span>.</td>
</tr>
<tr>
<td width="150">&amp;H002b</td>
<td>Specifies the folder that contains the components shared across applications. A typical path is <span class="Monospace">C:\Programs\Common</span>. Valid only for Windows NT, Windows 2000, and Windows XP systems. Not valid for Windows Millennium (Windows Me).</td>
</tr>
<tr>
<td width="150">&amp;H0002</td>
<td>Specifies the folder that contains the user program groups. A typical path is <span class="Monospace">C:\Documents and Settings\username\Start Menu\Programs</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0008</td>
<td>Specifies the folder that contains the most recently used documents. A typical path is <span class="Monospace">C:\Documents and Settings\username\Recent</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0009</td>
<td>Specifies the folder that contains <span class="Monospace">Send to</span> menu objects. A typical path is <span class="Monospace">C:\Documents and Settings\username\SendTo</span>.</td>
</tr>
<tr>
<td width="150">&amp;H000b</td>
<td>Specifies the folder that contains the start menu objects. A typical path is <span class="Monospace">C:\Documents and Settings\username\Start Menu</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0007</td>
<td>Specifies the folder that contains the autostart group. A typical path is <span class="Monospace">C:\Documents and Settings\username\Start Menu\Programs\Startup</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0025</td>
<td>Specifies the Windows system folder. A typical path is <span class="Monospace">C:\Windows\System32</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0015</td>
<td>Specifies the folder that contains the templates. A typical path is <span class="Monospace">C:\Documents and Settings\username\Templates</span>.</td>
</tr>
<tr>
<td width="150">&amp;H0024</td>
<td>Specifies the Windows folder SYSROOT. The SYSROOT folder corresponds with the environment variables <span class="Monospace">%windir%</span> or <span class="Monospace">%SYSTEMROOT%</span>. A typical path is <span class="Monospace">C:\Windows</span>.</td>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String variable</a> type.</td></tr>
</table>
</div>

## Python example

```python
CSIDL_ADMINTOOLS= 0x0030
CSIDL_ALTSTARTUP              = 0x001d
CSIDL_APPDATA                 = 0x001a
CSIDL_BITBUCKET               = 0x000a
CSIDL_CDBURN_AREA             = 0x003b
CSIDL_COMMON_ADMINTOOLS       = 0x002f
CSIDL_COMMON_ALTSTARTUP       = 0x001e
CSIDL_COMMON_APPDATA          = 0x0023
CSIDL_COMMON_DESKTOPDIRECTORY = 0x0019
CSIDL_COMMON_DOCUMENTS        = 0x002e
CSIDL_COMMON_FAVORITES        = 0x001f
CSIDL_COMMON_MUSIC            = 0x0035
CSIDL_COMMON_PICTURES         = 0x0036
CSIDL_COMMON_PROGRAMS         = 0x0017
CSIDL_COMMON_STARTMENU        = 0x0016
CSIDL_COMMON_STARTUP          = 0x0018
CSIDL_COMMON_TEMPLATES        = 0x002d
CSIDL_COMMON_VIDEO            = 0x0037
CSIDL_CONTROLS                = 0x0003
CSIDL_COOKIES                 = 0x0021
CSIDL_DESKTOP                 = 0x0000
CSIDL_DESKTOPDIRECTORY        = 0x0010
CSIDL_DRIVES                  = 0x0011
CSIDL_FAVORITES               = 0x0006
CSIDL_FONTS                   = 0x0014
CSIDL_HISTORY                 = 0x0022
CSIDL_INTERNET                = 0x0001
CSIDL_INTERNET_CACHE          = 0x0020
CSIDL_LOCAL_APPDATA           = 0x001c
CSIDL_MYDOCUMENTS             = 0x0005
CSIDL_MYMUSIC                 = 0x000d
CSIDL_MYPICTURES              = 0x0027
CSIDL_MYVIDEO                 = 0x000e
CSIDL_NETHOOD                 = 0x0013
CSIDL_NETWORK                 = 0x0012
CSIDL_PERSONAL                = 0x0005
CSIDL_PRINTERS                = 0x0004
CSIDL_PRINTHOOD               = 0x001b
CSIDL_PROFILE                 = 0x0028
CSIDL_PROFILES                = 0x003e
CSIDL_PROGRAM_FILES           = 0x0026
CSIDL_PROGRAM_FILES_COMMON    = 0x002b
CSIDL_PROGRAMS                = 0x0002
CSIDL_RECENT                  = 0x0008
CSIDL_SENDTO                  = 0x0009
CSIDL_STARTMENU               = 0x000b
CSIDL_STARTUP                 = 0x0007
CSIDL_SYSTEM                  = 0x0025
CSIDL_TEMPLATES               = 0x0015
CSIDL_WINDOWS                 = 0x0024

dd.MsgBoxDisp("Application Data Folder = " + dd.SHGetFolderPath(CSIDL_LOCAL_APPDATA))
```

---

*Source: `ComOff/SHGetFolderPath.htm`*
