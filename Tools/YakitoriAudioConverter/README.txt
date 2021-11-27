Yakitori Audio Converter - Convert fuz-xwm-wav-various audio files
Version 1.4
by BowmoreLover
https://www.nexusmods.com/skyrim/mods/73100
https://www.nexusmods.com/skyrimspecialedition/mods/17765
https://www.nexusmods.com/fallout4/mods/9322


CONTENTS

1. Introduction
2. Motivation and purpose
3. Major features
4. Supported file format
5. Requirements
6. Install
7. Uninstall
8. How to use
9. Notes / Limitation / Known issues
10. Credits & Special Thanks


====================================================================================================================
 1. Introduction
====================================================================================================================

This tool is "Yet Another" audio converter. By default, you can convert between fuz, xwm and wav files. By separately download and install the following tools, you can convert to/from various audio files such as mp3, and convert from various video files such as mp4 and wmv: LAME, FFmpeg
Also you can convert audio files from bsa/ba2 directly. Just drop bsa/ba2 files to the tool window.

ENJOY!


What's Yakitori?
Yakitori (Japanese: 焼き鳥) is a Japanese type of skewered chicken. Google image seach here: https://www.google.com/search?q=yakitori&tbm=isch
At first the name of this tool was "Yet Another Audio Converter". However, I noticed that there was already a tool with the same name and decided to think about another name to avoid confusion. Then I went to a izakaya(Japanese pub) and ordered some beer and Yakitori, and suddenly I came up with the idea, so naming it to Yakitori (no sense but I wanted to name the beginning with "Y" lol).


For Japanese users: Japanese guide now available.
日本のユーザへ： 日本語の利用ガイドがこちらにあります => http://thinkingskeever.hatenablog.com/entry/2016/02/02/191802


====================================================================================================================
 2. Motivation and purpose
====================================================================================================================

I'm offten convert fuz files to wav/mp3 format and editing with Audacity or playback with Media Player. For this kind of work, Skyrim Audio Converter by JohnB https://www.nexusmods.com/skyrim/mods/8303/ met comparative requirements. I was using all the way this tool but sometimes bit unstable in my PC and I wanted to specify more conversion parameters, so I decided to develop this tool. I want to emphasize that Skyrim Audio Converter gave me a big inspiration on developing this tool. Many thanks JohnB!

With other similar tools in NexusMods, the flow of conversions is hidden and it is not clear which option will affect which external tool. This is useful for simplifying UI and ease of use, but It may be difficult to deal with conversion errors because the parameters of external tools cannot be tweaked. So I designed the conversion flow and the parameters of the external tool clearly, and designed to be able to choose conversion options for each external tool. You may think that this is too complicated but do not worry. Basically you can convert with default option.


====================================================================================================================
 3. Major features
====================================================================================================================

Select files to convert:
- You can select audio files to convert from menu or drag and drop. Selected files will be added to the file list.
- You can select single files, folders and bsa/ba2 files.
- Use the check box of the file list, you can choose the file you want to convert.

Convert audio files:
- By default, you can convert between fuz, xwm and wav (Lip files can be handled together).
- If you install LAME, you can convert between wav and mp3.
- If you install FFmpeg, you can convert between wav and various audio file formats (mp3, ogg, flac, aiff, etc.).
- If you install FFmpeg, you can convert from various video formats (avi, flv, mpg, mp4, etc.).
- Converted files can be output to the same as input folder, or the specified folder.
- If you select the "Create subfolders" option, the folder hierarchy of the input file will be re-created in the output folder. Note that "Subfolder" will determined based on the opened folder or BSA path, so this function does not work when opening individual files.
- You can choose a variety of conversion options. Don't worry though you may feel a bit complicated. Basically, it can be converted by the default settings.
- Merging audio and lip files into Fuz is very easy. Just place a lip file with the same name in the folder with the audio file.

User Interface:
- Convenient file list (maybe!). Audio files are categorized depending on the status. The list displays useful information, such as the result of the conversion or the presence of a lip file. Also, you can sort by clicking on the column header.
- From the right-click menu of the file list, you can open input/output files, input/output folders and bsa/ba2 files.
- All of the settings are saved to INI file and will be carried over to the next startup.
- You can show the command help of LAME and FFmpeg from the Help menu. You don't need to open command prompt for reading help message. It should help to specify the additional arguments on the conversion option.
- Multi-language support. Currently supports English and Japanese. If you are interested in translating UI please contact me.

Notes:
- Conversion is parallelized in multi-process and multi-thread. The default parallel number depends on the number of logical processors in your CPU. You can change the parallel number in the UI.
- Opening a large number of files, especially the bsa that contains a large number of voice files, will slow down the UI. There should be no impact on the speed of conversion, so be patient. If you just want to look for an actors voice and extract it, try my another tool Lazy Voice Finder : https://www.nexusmods.com/skyrim/mods/82482/


====================================================================================================================
 4. Supported file format
====================================================================================================================

Input file format (audio):
- fuze (.fuz)
- xwma (.xwm)
- wave (.wav) - LAME or FFmpeg required
- mp3 (.mp3) - LAME or FFmpeg required
- ogg (.ogg/.oga) - FFmpeg required
- flac (.fla/.flac) - FFmpeg required
- aiff (.aif/.aiff) - FFmpeg required
- wma (.wma) - FFmpeg required
- mp4 audio (.m4a) - FFmpeg required

Input file format (video):
- asf (.asf) - FFmpeg required
- avi (.avi) - FFmpeg required
- flv (.flv) - FFmpeg required
- mov (.mov/.qt) - FFmpeg required
- mp4 (.mp4) - FFmpeg required
- mpeg (.mpg/.mpeg) - FFmpeg required
- ogg (.ogv/.ogx) - FFmpeg required
- web-m (.webm) - FFmpeg required
- wmv (.wmv) - FFmpeg required

Output file format:
- fuze (.fuz)
- xwma (.xwm)
- wave (.wav) - LAME or FFmpeg required
- mp3 (.mp3) - LAME or FFmpeg required
- ogg (.ogg/.oga) (flac/opus/speex/vorbis compression) - FFmpeg required
- flac (.fla/.flac) - FFmpeg required
- aiff (.aif/.aiff) - FFmpeg required


====================================================================================================================
 5. Requirements
====================================================================================================================

Required:

- Windows 7 or later
- Microsoft .NET Framework 4.6.1 or later
I don't have a windows XP/7/8 so it doesn't work verification, but perhaps it works well if .NET Framework installed.


Optional (for more audio file formats):

- LAME 3.99.5 or later (http://lame.sourceforge.net/)
Required in order to handle mp3 files. But not required If there is FFmpeg.
You can download compiled binaries from RAREWARES http://www.rarewares.org/mp3-lame-bundle.php
32bit version or 64bit version, either one is OK. 

- FFmpeg 2.8.5 or later (http://ffmpeg.org/) 
Required in order to handle various audio/video files.
You can download compiled binaries from Zeranoe FFmpeg http://ffmpeg.zeranoe.com/builds/
32-bit static version or 64-bit static version, either one is OK.


====================================================================================================================
 6. Install
====================================================================================================================

Download zip file and extract zip to any folder (Recommended other than "Program Files" folder and Bethesda game folder).

The optional external tools (lame.exe, ffmpeg.exe), please copy into the installation folder.

NOTE: In version 1.4, the configuration of the installation folder has been changed. To upgrade from a version earlier than version 1.4, please clear the installation folder before installing.


====================================================================================================================
 7. Uninstall
====================================================================================================================

Delete the installed files and folders. Registry does not used.


====================================================================================================================
 8. How to use
====================================================================================================================

How to conversion:

(0) Launch YakitoriAudioConverter.exe

(1) Select input format.

(2-a) Add audio files you want to convert by "File" menu or Drag and Drop.

(2-b) You can also choose files by checkbox.

(3) Select output format.

(4) Select output folder.

(5) (Optional) Select encoder/decoder settings. The displayed options depends on input/output type. If you don't know exactly what you do, just leave the default value.

(6) Press "Convert" button to start conversion.

(7) When conversion is finished, file list is categorized by conversion result. If it can not be converted, an error message is output to the log. You can see errors for each files by "Show file status" menu on the right-click menu.


Shortcut keys and Convenient operations:

(Main Window)
Ctrl+O : Open files
Ctrl+L : Open folders
F5 : Convert

(File List)
DEL : Delete selected rows
Ctrl+A : Select all rows
Ctrl+C : Copy file name to clipboard
Ctrl+G : Toggle grouping
Alt+Up : Jump to previous group
Alt+Down : Jump to next group
Shift+Click : Range selection
Drag the margin : Range selection
Click group title : select all files in the group
Double Click group title : Collapse/Expand group
Range selection and click checkbox : Check/Uncheck selected all files
Click column header : Select sort column, Change sort order
Hover mouse cursor to File name : Show file name by tool tip
Hover mouse cursor to Status : Show detailed results by tool tip (error message, created files, etc.)
Right Click : Show context menu
Double Click file : Open input file
Double Click the "Converted" in the status column : Open output file

(Option Window)
Hover mouse cursor to input/output file type : Show file extensions

(Log Window)
Ctrl+A : Select all
Ctrl+C : Copy
Right Click : Show context menu

(Status Bar)
Click group name : Jump to group


====================================================================================================================
 9. Notes / Limitation / Troubleshooting
====================================================================================================================

- There may be a bug in this tool. Please be sure to MAKE A BACKUP of the original audio files. 

- The result of the conversion depends on the external tool. If a conversion error occurs, look at the message of the external command contained in the errpr message.

- The number of rows in the Log window can affect performance. Please clear it regularly.

- ListView of .NET (in particular grouping feature) is very slow and buggy, so I was as much as possible tweak and tuning. If the file list is no longer being re-drawn, just show "About" dialog (Help - About menu) to reset. If such a problem occurs frequently, please report to me.

- You can enjoy the converted file freely, but please pay attention to the copyright of the original music and video when distributing or publishing to the public.

- Errors on encoding xwm : "Error: Unable to convert sound file. External command xWMAEncode.exe error. ExitCode: -2147221501"
  This error is caused by Microsoft xWMAEncoder and occurs when the file size exceeds the upper limit. You have to reduce the audio file size by lower the sampling frequency of the audio file or reduce the bitrate option of xWMAEncoder. The way to convert is as follows:
  (If you want to convert from wav file, once converted to aif format)
  1. Input Format: Select "audio files (ffmpeg)". If there is no item, please install ffmpeg.exe in the Yakitori folder.
  2. ffmpeg generic audio decoder settings / Sampling frequency: Select 22.05KHz
  3. xWMAEncode xwm encoder settings / Bitrate : Select 32kbps
  4. Do convert
  5. If no luck, try lowering the sampling frequency and bitrate. 

- Errors on decoding xwm : "Unable to convert sound file. External command xWMAEncode.exe error. ExitCode: -2147024809 ... ERROR: Input file type is neither PCM nor xWMA"
  Perhaps the fuz (xwm) file is in PS3 format. 

- Errors on decoding xwm : "Unable to convert sound file. External command xWMAEncode.exe error. ExitCode: -2003238911 ... ERROR: Requested audio format unsupported: format tag must be WAVE_FORMAT_PCM or WAVE_FORMAT_IEEE_FLOAT"
  Perhaps the fuz (xwm) file is in PS4 format.


====================================================================================================================
 10. Credits & Special Thanks
====================================================================================================================

=== Libraries/tools ===

LZ4 for .NET https://github.com/IonKiwi/lz4.net
Copyright(c) 2016, IonKiwi
Copyright(c) 2011-2014, Yann Collet, All rights reserved.

Microsoft (R) xWMA Encoding Tool Copyright (C) 2009 Microsoft Corporation. All rights reserved.

=== Special Thanks ===

JohnB for his Skyrim Audio Converter https://www.nexusmods.com/skyrim/mods/8303/
    His work gave me a big inspiration on developing this tool. Many thanks!
Unofficial Elder Scrolls Pages for mod file format refference http://www.uesp.net/wiki/
    The information on this page is very helpful to me.
AFK Mods forum for informations of plugin file format https://afkmods.iguanadons.net/
    The discussion on the file format on this forum was very useful to me.
And, thanks for all over the modding community, Nexus Mods, Bethesda and YOU!

=== Development tools ===

Microsoft Visual C# 2015
GIMP (edit screen shots)
LibreOffice

//