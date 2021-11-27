Lazy Voice Finder - Fidn voice assets just you want
Version 1.3.7
by BowmoreLover

Official Sites:
- NexusMods Oblivion http://www.nexusmods.com/oblivion/mods/47801/
- NexusMods Fallout 3 http://www.nexusmods.com/fallout3/mods/22552/
- NexusMods Fallout New Vegas http://www.nexusmods.com/newvegas/mods/63317/
- NexusMods Skyrim http://www.nexusmods.com/skyrim/mods/82482/
- NexusMods Skyrim Special Edition http://www.nexusmods.com/skyrimspecialedition/mods/8619/
- NexusMods Fallout 4 http://www.nexusmods.com/fallout4/mods/24309/

Supporters Sites:
- Gamer Mods (Russian) http://gamer-mods.ru/load/tes_v_skyrim/instrumentarij/lazy_voice_finder/59-1-0-5701
- Skyrim Mod Database (Japanese) http://skyrim.2game.info/detail.php?id=82482
- Skyrim Special Edition Mod Database (Japanese) http://skyrimspecialedition.2game.info/detail.php?id=8619
- Fallout4 Mod Database (Japanese) http://fallout4.2game.info/detail.php?id=24309

===================================================================================================================
CONTENTS

1. Introduction
2. Motivation and purpose
3. Major features
4. Requirements
5. Install
6. Uninstall
7. The most basic usage
8. Notes / Limitation / Known issues
9. Feature plans
10. My other tools
11. Credits & Special thanks


===================================================================================================================
 1. Introduction
===================================================================================================================

Hi there.

This is a tool for mod authors and translators who handle voice files. You can list the voice files of vanilla/mods and search by various conditions such as dialogue text or voice type. You can play/edit(*1)/extract voice files directly without extracting BSA/BA2 files or FUZ files in advance. Oblivion/FO3/FNV/Skyrim LE/Skyrim SE/FO4 are supported. Of course it supports Skyrim SE's new BSA file format and Fallout 4's BA2 file format.

Typical uses are as follows:
- Find voice files of vanilla/mods to edit custom voice.
- Check your own custom voiced mod voice files for unnecessary / lacking.
- Just enjoy dialogues and voices. Vanilla has unused hidden dialogues and voices, it will be fun to find this.

I hope this will be of your help.

(*1) Since it is extracted to a temporary folder and edited, so not possible to directly edit and update the voice file in the Data folder or BSA/BA2 file. 


=========================================================
 Greeting to Oblivion/Fallout3/Fallout NV community
=========================================================

I'm very pleased to have released this tool to the new communities.
Originally I developed this tool for Skyrim. I thought this tool would be useful in other Bethesda games, so decided to support Oblivion/FO3/FNV.
I have played Oblivion quite a long time ago but I don't know the modding situation recently and I have not played FO3/FNV yet. So there should be something wrong, please do not hesitate to let me know.


===================================================================================================================
 2. Motivation and purpose
===================================================================================================================

Recently I had voice-file translation of Skyrim mods that using vanilla's voice (eg. Skyrim mod Minerva - Custom High Elf Voiced Follower (http://www.nexusmods.com/skyrim/mods/74256/) by cloudedtruth and rxkx22). The most troublesome thing in this task is finding what we want from vanilla's voice files.
For this type of work, Voice File Reference Tool by greentea101 (http://www.nexusmods.com/skyrim/mods/28462/) is fairly convenient and it can find voice file names from dialogue text. However, in order to handle voice files, we need to extract BSA file and locate the voice files. It also requires the creation of a dictionaries for tools, and we can not search other than vanilla's voices.
This tool is an attempt to solve the above problem.

Although, greentea101's tool was very useful for me, and gave me a big inspiration on developing this tool. Thanks a lot!

Additional notes:
After releasing this tool, I learned that FO4 Voice File Reference Tool (http://www.nexusmods.com/fallout4/mods/12132/) was already released and it can be play/extract voice files from ba2/fuz. Awesome! VFRT is the best choice if you are FO4 modder and enough to be able to search from vanilla/DLC. If I knew this I may not have developed this tool but it's too late.
The concept of VFRT and this tool is very different. Although VFRT features fast search by dictionary file and very easy to use, it can not open any plugins Immediately. This tool can be opened with any plugin, but the search performance is not very good and it's a bit complicated.
As with any tool, the important thing is to use all the tools according to your application.


===================================================================================================================
 3. Major features
===================================================================================================================

Supported games:
- Oblivion
- Fallout 3
- Fallout New Vegas
- Skyrim Legacy Edition (Skyrim LE)
- Skyrim Special Edition (Skyrim SE)
- Fallout 4
- Fallout 76 (Experimental)

Multilingual support:
- UI languages:
  - English
  - Japanese
  - Russian  (Translation by anizorda http://gamer-mods.ru/index/8-16387)

  Now available UI translation resource files here (see Misc. section) : http://www.nexusmods.com/skyrim/mods/82482/
  You can freely translate resource file and redistribute it. (Please note that you still can NOT redistribute the main file.)
  I would appreciate it if you could send translation file to me (author), I will bundle to the main file and credit translator's name.

- Plugin languages (Requests are welcome):
  Arabic, Baltic, Chinese, Czech, Danish, English, Finnish, French, German, Greek, Hebrew,
  Hungarian, Italian, Japanese, Korean, Norwegian, Polish, Portuguese, Russian, Spanish(Spain/Mexico), 
  Swedish, Thai, Turkish, Vietnamese
  You can select any language or code page by "Custom" language menu.
  You can also add any language or code page to Data/GameLang_*.txt file. See the comments in the file.

- Notes for Oblivion/FO3/FNV users:
  - Oblivion/FO3/FNV doesn't support multiple languages, so you can view only one language at once.
  - Oblivion/FO3/FNV is officially localized to only a few languages, therefore localized to other languages by mods. However I don't know what languages are localized by mods and which code page is used in each language. So if you are using mods to localization, you need to change the code page in Data/GameLang_*.txt according to mods. I'm very interested in this information so I would appreciate it if you let me know.

Supported voice file formats:
- Oblivion: mp3/lip
- Fallout 3/Fallout NV: ogg/lip
- Skyrim LE/Skyrim SE/Fallout 4/Fallout 76: fuz/xwm/wav/lip

Plugins selection:
- You can choose the plugin to load from the plugin list of the game.
- You can load any plugin files other than the Data folder. You can also load plugin files with drag-and-drop.
  There is an option to automatically select the game mode by plugin type to open.

Convenient Spreadsheet:
- You can following operations like Excel or OpenOffice:
  - Sort rows.
  - Filtering by text or checked items.
  - Hide/unhide columns.
  - Change column positions.
- The spreadsheet has the following columns. You can hide/unhide any of them according to your preference:
  - State : The following information / warnings. Although it is an icon display, text can be displayed with a tool tip.
    - Bad File Name : Non-standard voice file name.
    - Bad File Path : Non-standard voice file path.
    - Overridden : Overridden with voice file of the same name according to the rules of the game engine.
    - No Dialogue : Corresponding dialogue response record (INFO) not found.
    - No Text : Dialogue text can not be found in STRINGS file (rare case).
    - No Strings File : Localized plugin's STRINGS file is missing.
    - No Voice File : Voice file corresponding to dialogue response record (INFO) is not found.
    - Master Record Reference : Refer to master plugin's dialogue response record (INFO).
  - Index : Plugin's load order.
  - Plugin : Plugin name.
  - Last Modifier : Plugin name that last modified the dialogue response record (INFO).
  - FormId : Form Id of dialogue response record (INFO)
  - FormId without Load#  : Form Id of dialogue response record (INFO) - Load order not included (ie always starts with "00").
  - Response Num : Response number of dialogue response record (INFO).
  - Edid : Editor Id of dialogue response record (INFO).
  - Topic FormId : Form Id of dialogue topic record (DIAL).
  - Topic Edid : Editor of dialogue topic record (DIAL).
  - Topic Text : Text of dialogue topic record (DIAL).
  - Quest FormId : Form Id of the associated quest.
  - Quest Edid : Editor Id of the associated quest.
  - Quest Name : Name of the associated quest.
  - Category/Subtype
    - Dialogue category : Topic/Favor/Scene/Combat/Favors/Detection/Service/Misc/etc...
    - Dialogue subtype (DIAL:SNAM) : Attack/PowerAttack/Hello/Goodbye/etc... (will be blank in TES4/FO3/FNV)
  - Emotion : Emotion - Neutral/Anger/Disgust/Fear/Sad/Happy/Surprise/Puzzled/etc...
  - Conditions : Conditions of dialogue response record (INFO). NPC/location/player's gender condition will be displayed but incomplete.
  - Bsa Name : BSA/BA2 file name for storing voice files or "Loose".
  - Full Path : Full path of voice files.
  - Base Path : Full path of Data folder or BSA/BA2 file.
  - Path : Relative path from Data folder.
  - File Name : Voice file name.
  - Extensions : Voice file extensions. - fuz/xwm/wav/lip/ogg/mp3
  - Voice Type : Voice type.
  - Script Notes : Script notes (INFO:NAM2). This text is not localized and remains in English.
  - Edits : Edits (INFO:NAM3). This text is not localized and remains in English.
  - Prompt : Prompt of dialogue (INFO:RNAM), known as 'Prompt override' in Skyrim. In dialogue option of FO4, Topic Text (DIAL:FULL) is rarely used, seems to be replaced with Prompt. For FO4, please use the Prompt column instead of the Topic Text column.
  - Dialogue 1 : Dialogue text. You can choose any language in Settings dialog.
  - Dialogue 2 : Dialogue text (Optional). You can choose any language in Settings dialog.
  - Keyword : Available on Fallout 4 / Fallout 76 only. Keywords of such as AO_Comment, CAT_CustomEvent or CAT_Event (DIAL:KNAM, a mechanism for providing a keyword indicating a specific situation to a companion).
  - StringId : String Id of dialogue text.

Search voice files:
- Search target:
  - Dialogue Text
  - Form Id
  - Edid
  - File Name
- Search mode:
  - Partial matching
  - Reguar expression
  - And search : Search with the AND condition of the text delimited by a space. To specify text that includes spaces, enclose it in quotation marks (").
  - Or search : Search with the OR condition of the text delimited by a space. To specify text that includes spaces, enclose it in quotation marks (").
  - Prefix matching
  - Suffix matching
  - Exact matching
- Search options:
  - Match case
  - Match word : For example, you can prevent "Goodbye" from hitting even if you search by "bye".
- Auto complete is available for text search box. Auto complete based on actual data of search target column. You can toggle this option in the options menu.
- Record up to 40 search histories. You can recall with a drop-down of the text search box.

Operate voice files:
  - Play sound : You can cancel playback with Pause key or tool button.
  - Edit sound : You can edit voice file with Audacity (or the other sound editor).
    You can also open a file renamed with dialogue text. You can enable this option in settings dialog.
  - Open Extracted Folder : Extract/copy the voice files to a temporary folder and convert FUZ/XWM/MP3/OGG to WAV automatically. The LIP file will also be extracted/copied.
    You can also extract a file renamed with dialogue text. You can enable this option in settings dialog.
  - Open Source Folder : Open the folder containing the voice file. If the voice file is in the BSA/BA2 file, will open the folder containing the BSA/BA2 file.
  - Copy Voice File : You can copy the voice file to the clipboard. If there is a LIP file, copy it together.
  - Copy Voice File as WAV Format : You can copy the voice file to the clipboard as WAV format. LIP files are not copied.
  - Rename and Copy Source File with Clipboard Text : Rename the voice file with the text in the clipboard and copy it to the clipboard. If there is a LIP file, copy it together.
  - Copy Selected Text : Copy the text in the selected cells to the clipboard. Multiple selection is supported.
  - Copy File Names of Selected Rows : Copy the voice file name of the selected rows to the clipboard. Multiple selection is supported.
  - Copy Asset Paths of Selected Rows : Copy the voice asset path of the selected rows to the clipboard. Multiple selection is supported.
  - Export Files of Selected Rows : Export audio files of the selected rows to '<Install folder>/Export' folder. Files are always overwritten. You can cancel the export process with the 'Pause' key. Since it is unexpected to use exporting in large quantities, please use other tools such as Yakitori Audio Converter.

Search by Clipboard:
- Automatically search with the text copied to the clipboard. You can toggle this option in the options menu.
- It may be handy when used with xEdit or xTranslator.
- The search target is automatically switched according to the format of the copied text as follows:
  - Start with Form Id : Form Id
  - Start with Form Id enclosed in '[]' : Form Id
  - Editor id enclosed in '<>' : Edid
  - End with voice file extensions : File Name
  - The other case : Dialogue 1 or Dialogue2 (the last selected one)

Miscellaneous features:
- You can choose rows height : Auto / 1 - 5 line(s)
- You can lock the tool's window to the top-most in Options menu.
- You can choose whether the columns fit to the window width in the options menu.
- You can export the currently displayed record to a CSV file. Choose the option that suits your spreadsheet application in the export CSV dialog.
- You can reopen recently used files from the "File - Recent Files" menu.
- You can reload the currently opened file using "Reload files" button.

===================================================================================================================
 4. Requirements
===================================================================================================================

Required:
- Windows 7 or later (Tested on Windows 10)
- Microsoft .NET Framework 4.6.1 or later (https://www.microsoft.com/en-us/download/details.aspx?id=49981)
- Microsoft Visual C++ 2010/2015/2017 Redistributable Packages:
  Please install x64 to use LazyVoiceFinder.exe(64-bit), x86 to use LazyVoiceFinder32.exe(32-bit).
  - Microsoft Visual C++ 2010 Redistributable Package (x86) (https://www.microsoft.com/en-us/download/details.aspx?id=5555)
  - Microsoft Visual C++ 2010 Redistributable Package (x64) (https://www.microsoft.com/en-US/download/details.aspx?id=14632)
  - Microsoft Visual C++ 2015 Redistributable Update 3 (https://www.microsoft.com/en-US/download/details.aspx?id=53587)
  - Visual C++ Redistributable for Visual Studio 2017 (https://www.visualstudio.com/downloads/)
- Base Games (Oblivion/Fallout 3/Fallout New Vegas/Skyrim LE/Skyrim SE/Fallout 4/Fallout 76, DLC is option)
  !!! Please start the game once in Bethesda's launcher. Otherwise the tool can not detect the installation folder of the game. You can explicitly set the installation folder of the game in the settings dialog. !!!

I don't tested on windows XP/Vista/7/8, but should works well if .NET Framework 4.6.1 installed.

Optional:
- Audacity (http://www.audacityteam.org/)
  It is necessary for editing the voice file. I'm using Version 2.1.2 but should work with different version, and should work with the other sound editors, but I have not tested it.

Optional(for Skyrim):
- Multiple Languages Strings Unified Central by Francisco Pozo - DJ FrANKy EHP (http://www.nexusmods.com/skyrim/mods/82578/?)
- Multiple Languages Strings Unified Central SSE by Francisco Pozo - DJ FrANKy EHP (http://www.nexusmods.com/skyrimspecialedition/mods/4505/?)
  If you are looking for strings files in other languages, you can find them here.
  Note that as the strings file name of some languages is English, renaming it to the proper language name when used with this tool.

Optional(for Japanese languages, using Migemo feature):
- C/Migemo for Windows 32bit Version 1.3 (https://www.kaoriya.net/software/cmigemo/)


===================================================================================================================
 5. Install
===================================================================================================================

Download archive file and extract to any folder.
Must be sure not to Windows/Program Files/Game installation folder.

When updating from the old version, basically simply overwrite it.
However, the file structure changed significantly in v1.2.0. When updating from version before v1.2.0, recommended to install it in a clean folder.

Note: Since v1.3.0, the required version of .NET Framework has been changed to 4.6.1. If the tool can not be started upgrade the .NET Framework from the url written in the Requirements section.


===================================================================================================================
 6. Uninstall
===================================================================================================================

Delete the installed files and folders. Registry does not used.


===================================================================================================================
 7. The most basic usage
===================================================================================================================

=== Launch & plugin selection ===

- Launch LazyVoiceFinder.exe
  To start up from a 32-bit program like the old Mod Organizer, launch LazyVoiceFinder32.exe.
- Select the game from "Game Mode" menu (Oblivion / Fallout 3 / Fallout NV / Skyrim LE / Skyrim SE / Fallout 4 / Fallout 76).
- Press "Open" button.
- Select the plugins you want to open. You can select only the vanilla+DLC plugins by pressing "Select None" and "Select Vanilla + DLC" button. Finally press the "OK" button.
- After waiting for a while, the list of voice files is displayed into spreadsheet. If there is a corresponding dialogue record, the dialogue text will also be displayed.

=== Text search ===

- You can search by entering text in the search text box. The default search target is "dialogue 1", you can change the target with the left combo box.

=== Voice file operation ===

To operate voice files right-click the spreadsheet rows to display the operation menu.

- "Play Sound" : Play the voice file.
- "Edit Sound" : Edit the voice file. If you can not select the menu, set the path of the sound editor in the Settings dialog.
- "Open Extracted Folder" : Extract/ copy the voice files to a temporary folder and convert FUZ/XWM/MP3/OGG to WAV automatically. The LIP file will also be extracted/copied.
- "Open Source Folder" : Open the folder containing the voice files. If the voice file is in the BSA/BA2 file, will open the folder containing the BSA/BA2 file.

=== Sorting, Filtering & Customize spreadsheet ===

- You can do something like Excel or OpenOffice.
- Sort : Click the column header. The sort direction is toggled each click.
- Filtering : Click the arrow button on the column header, a filtering menu will appear.
- Unfiltering : Right-click the column header, a column menu will appear. 
- Change column position : Drag the column header.
- Hide / unhide columns : Right-click the column header, a column menu will appear.

=== Changing the dialogue language ===

- Select "Options - Game Specific Settings" menu and open each game page. You can choose up to two languages of dialogue.
  Reopening the plugin will apply the selected language.
  Please note that even if you select a language, it will not display correctly unless there is a corresponding strings file (Substitute in English).

=== Shortcut Keys and Convenient operations ===

(Main window)
F5 : Open plugins
F9 : General Settings
F10 : Game Specific Settings
Ctrl+F1 : Game mode - Oblivion
Ctrl+F2 : Game mode - Fallout 3
Ctrl+F3 : Game mode - Fallout New Vegas
Ctrl+F4 : Game mode - Skyrim Legacy Edition
Ctrl+F5 : Game mode - Skyrim Special Edition
Ctrl+F6 : Game mode - Fallout 4
Ctrl+F7 : Game mode - Fallout 76
ESC/F2 : Focus to search text box
Enter : Text search
Ctrl+Enter : Toggle search target between "Dialogue 1" and "Dialogue 2", and text search
Ctrl+1 ~ Ctrl+5 : Change search target
Alt+N/Alt+E/Alt+A/Alt+R/Alt+P/Alt+S : Change search mode
Alt+Down : Show search histroy
Pause : Stop audio / Cancel search

(Spreadsheet)
Right-click/Menu key : Show voice operation menu
Enter/Space/Ctrl+P/Double-click : Play the voice file (toggle)
Ctrl+E : Edit the voice file
Ctrl+O : Open extracted folder
Ctrl+A : Select all cells
Ctrl+C : Copy cell text
Ctrl+Shift+C : Copy voice file
Alt+Up/Alt+Down : Show filter menu
Right-click : Show voice file operation menu
Click top-left cell : Show top-left menu and you can reset all filters

(Log Window)
Ctrl+A : Select all
Ctrl+C : Copy
Right-click : Show log menu


===================================================================================================================
 8. Notes / Limitation / Known issues
===================================================================================================================

- When editing the voice files and redistributing it, be sure to get permission from author.

- Even vanilla voice files should have certain restrictions on redistribution. Generally should not possible to use vanilla voice files for other game mods (Even if game of Bethesda). Please check EURA of games/CK when using asset of vanilla.

- There may be a bug in this tool. Please be sure to MAKE A BACKUP of the original game files or mods files.

- Bad English. I'm not an English native speaker. Improvement suggestion of the sentences is a welcome.

- Processing time depends on the number of plugin/voice files.

- The value of the condition column is incomplete. Only a few conditional expressions can be recognized, and can't recognize an alias. It should only be kept in mind as reference.

- At the moment, I'm implementing it assuming that all records have different form id (Ie there is no form id duplication).
  In some plugins like Enderal, another dialogue response record may have the same form id.
  For example of Enderal (Version around 2016/8), different dialogue responses have the same form id "00096693"
    [00] Skyrim.esm \ Dialog Topic \ 0009665E <MQ11c_Generic_YalKajshimTopic002> \ 00096693    "Danke."
    [00] Skyrim.esm \ Dialog Topic \ 00096675 <MQ11c_Generic_OlielTopic005> \ 00096693    "Take care, and enjoy your stay here. "
  In this case, some records are not displayed, and some records and audio files are not properly matched.
  The voice file name does not have a form id of dialogue topic, so it can not be simply matched with records. Although it can be solved in theory, but because it may slow down the performance it is left as it is.
  I will consider solutions if there are some requests.

- In some languages, there is a fact that the Creation Kit may crashes unless you convert the strings in the plugin to a local code page. For example in Japanese need to convert to Shift-JIS code page. If you want to open a plugin that have such a local code page, add the definition of Data/GameLang_*.txt file.


===================================================================================================================
 9. Feature plans
===================================================================================================================

- I will continue to bug fixes and improve operations for the time being.

- Suggestions and advice are welcome.

- There is a plan to make a simple tutorial page.


===================================================================================================================
 10. My other tools
===================================================================================================================

Let me introduce my tools that you might be interested in. If you are interested, please try it.

- Yakitori Audio Converter - Convert fuz-xwm-wav-various audio files (for all games)
  http://www.nexusmods.com/skyrim/mods/73100/?
  http://www.nexusmods.com/fallout4/mods/9322?
  A GUI-based sound conversion tool that supports many file formats such as fuz/xwm/wav/mp3/ogg. You can also convert audio from video.
  This tool is superior to other tools in terms of program stability and abundance/transparency of parameters for the conversion tool (lame, ffmpeg).
  Although you can open sound files in bsa directly, it currently support Oldrim's bsa format only. I'm planning to support all bsa/ba2 formats.

- TesvCheckEspFiles - Check the missing resource files (for SkyrimLE/SE)
  http://www.nexusmods.com/skyrim/mods/71112/?
  This utility checks whether a file used with esp file exists. Typically, mod is configured with esm/esp file and resource files such as the scripts/sounds/textures/meshes. If the resource file is missing, mod not work correctly, or the graphics does wrong. With this utility, you will be able to list the missing files.
  To be honest, that intention was bite off more than I can chew, so still unfinished. But it is enough to check some assets.

- TesvRefidPicker - Showing RefID of NPC (for SkyrimLE/SE)
  http://www.nexusmods.com/skyrim/mods/72356/?
  This utility showing the RefID of NPC. RefId and NPC's informations are listed in the spreadsheet.
  You can filtering rows, sort rows, reorder columns, hide/unhide columns. You can copy the console command for all NPCs which is listed to the clipboard.

- SSLXLTNtoXML - Translation File Converter (for SkyrimLE, for mod translators)
  http://www.nexusmods.com/skyrim/mods/77759/
  This tool convert to TESVTranslator's XML file from Skyrim String Localizer's SSLXLTN file. Since Skyrim String Localizer is no longer updated, it is useful for converting past translation files.

- TESVKanjiChecker (for SkyrimLE/SE/The Witcher 3, for Japanese modders/translators)
  http://www.nexusmods.com/skyrim/mods/66768/? (http://www.nexusmods.com/skyrim/mods/66768/?)
  In general, the Japanese Kanji there are more than 8000 kinds of characters. However, in vanilla of Skyrim Japanese edition, it can be used only 2300 kind of kanji characters. This tool checks the kanji characters that can not be used in the vanilla. It supports The Witcher 3 as an option file.

- Japanese Phonetic Text Converter - Convert dialogue text to romaji from kanji (for SkyrimLE/SE/Fallout4, for Japanese modders/translators)
  http://www.nexusmods.com/skyrim/mods/83033/?
  http://www.nexusmods.com/skyrimspecialedition/mods/9190/?
  http://www.nexusmods.com/fallout4/mods/23253/
  The Facial Animation Generator of the Creation Kit only supports some languages and can not generate Japanese LIP files.
  This tool converts Japanese dialogue response text into text that "Facial Animation (LIP) Generator" in Creation Kit can "pronounce".
  It is also possible to cooperate with the speech reading software SofTalk, and you can check the conversion result by speech reading (a feature for my bad eye).

- WinMerge Plugins for TES-FO-TW3 Modders (for SkyrimLE/SE/Fallout4/Witcher3, for modders)
  https://www.nexusmods.com/skyrim/mods/98565
  https://www.nexusmods.com/skyrimspecialedition/mods/27347
  https://www.nexusmods.com/fallout4/mods/40012
  WinMerge plugins for comparing mod files using WinMerge.


===================================================================================================================
 11. Credits & Special thanks
===================================================================================================================

Lazy Voice Finder Copyright(c) 2017-2018, BowmoreLover, All Rights Reserved.
Development by BowmoreLover. All of the program was coded myself by scratch expect following libiraries/tools.

=== UI Translation ===

Russian by anizorda (http://gamer-mods.ru/index/8-16387)
Great appreciation to all translators!

=== External libraries/tools ===

LZ4 for .NET (https://github.com/IonKiwi/lz4.net)
Copyright(c) 2016, IonKiwi
Copyright(c) 2011-2014, Yann Collet, All rights reserved.

NAudio (http://github.com/naudio/NAudio)
Copyright(c) 2001-2017, Mark Heath

NAudio.Vorbis (https://github.com/NAudio/Vorbis)
Copyright(c) 2015, Andrew Ward

NVorbis (https://github.com/ioctlLR/NVorbis)
Copyright(c) 2016, Andrew Ward

C/Migemo (http://www.kaoriya.net/)
Copyright(c) 2003-2007 MURAOKA Taro (KoRoN)

kanaxs ex C# (https://dobon.net/)
Copyright(c) 2011, DOBON! <http://dobon.net>, All rights reserved.

Microsoft (R) xWMA Encoding Tool Copyright (C) 2009 Microsoft Corporation. All rights reserved.

=== Special thanks ===

greentea101 for his Voice File Reference Tool (http://www.nexusmods.com/skyrim/mods/28462/)
    His work gave me a big inspiration on developing this tool. Thanks a lot!
Unofficial Elder Scrolls Pages for mod file format refference (http://www.uesp.net/wiki/)
    The information on this page is very helpful to me.
Akira Uchida for Oradano Mincho Font (http://www.asahi-net.or.jp/~sd5a-ucd/freefonts/Oradano-Mincho/)
    I'm using his beautiful font for the typography of icon.
Francisco Pozo - DJ FrANKy EHP for Multiple Languages Strings Unified Central
    Multiple Languages Strings Unified Central (http://www.nexusmods.com/skyrim/mods/82578/?)
    Multiple Languages Strings Unified Central SSE (http://www.nexusmods.com/skyrimspecialedition/mods/4505/?)
    His multilingual strings file was of great use in tool development and testing.
AFK Mods forum for informations of plugin file format (https://afkmods.iguanadons.net/)
    The discussion on the file format of Fallout 4 on the forum was very useful to me.
ElminsterAU and xEdit dev team
    TES4Edit (http://www.nexusmods.com/oblivion/mods/11536/)
    FO3Edit (http://www.nexusmods.com/fallout3/mods/637/)
    FNVEdit (http://www.nexusmods.com/newvegas/mods/34703/)
    TES5Edit (http://www.nexusmods.com/skyrim/mods/25859/)
    SSEEdit (http://www.nexusmods.com/skyrimspecialedition/mods/164/)
    FO4Edit (http://www.nexusmods.com/fallout4/mods/2737/)
    xEdit is an indispensable tool for research and understanding of plugin format. Incredible work!
And thanks for all over the modding community, Nexus Mods, and of course Bethesda.

=== Development tools ===

Microsoft Visual C# 2015 + .NET Framework 4.0/4.6.1
TES4Edit by ElminsterAU (http://www.nexusmods.com/oblivion/mods/11536/?)
FO3Edit by ElminsterAU (http://www.nexusmods.com/fallout3/mods/637/?)
FNVEdit by ElminsterAU (http://www.nexusmods.com/newvegas/mods/34703/?)
TES5Edit by ElminsterAU (http://www.nexusmods.com/skyrim/mods/25859/?)
SSEEdit by ElminsterAU and SSEEdit team (http://www.nexusmods.com/skyrimspecialedition/mods/164/?)
FO4Edit by ElminsterAU (http://www.nexusmods.com/fallout4/mods/2737/?)
GIMP (for edit graphical resources) (https://www.gimp.org/)
Audacity (http://www.audacityteam.org/)
ScreenToGif (for create animated GIF) (http://www.screentogif.com/)

//