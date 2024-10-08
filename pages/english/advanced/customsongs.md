---
title: Add Custom Songs to Rock Band 3 Deluxe
sidebar: english_sidebar
permalink: adv_customsongs
folder: english
tags: [advanced, english]
summary: "How to add custom songs to Rock Band 3."
---

## Introduction:

Custom songs for Rock Band 3 are generally made with only the Xbox 360 in mind. They exist as CON files that can be converted for PS3. This guide will show you how to convert these files to PKG files you can install on PS3.

<span style="font-size:xxx-large;">This guide is primarily focused on customs songs, do not attempt to run official RB content through the fixer.</span>

The main guide on page 2 will fix two major problems the PS3 has with customs that the 360 doesn't and should follow for every custom you add.
* Infinite loading from improper encryption
* Crash from too high-quality audio

### Requirements:
* A modded PS3 console (with a method of transferring files to it) or the [[RPCS3 emulator]](https://rpcs3.net/){:target="_blank"}
* [[An installation of Rock Band 3 Deluxe]](https://rb3dx.milohax.org/){:target="_blank"} (Optional but highly recommended)
* [[Nautilus version 4.8.4 or later]](https://nemosnautilus.com/nautilus/){:target="_blank"} (Previously known as C3 CON Tools/C3Tools)
	* [[Mirror Link]](https://github.com/trojannemo/Nautilus/releases/){:target="_blank"}
* [[Onyx Music Game Toolkit]](https://github.com/mtolly/onyxite-customs){:target="_blank"}

## Converting to Xbox 360 CONs to PS3/RPCS3 Format
1\. If you wish to convert official Xbox 360 DLC, skip to step 4, otherwise continue reading below:  
[[Download the songs of your choice from RhythmVerse]](https://rhythmverse.co/songfiles/game/rb3).

2\. Open Nautilus. and select `PS3 Converter` on the home screen.  
![A screenshot of Nautilus. A cursor hovers over "PS3 Converter."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilushomeps3.png "Nautilus")

3\. Select `One-Click Batch PS3 Fixer` from the `Tools` menu. After the splash screen, navigate to the folder where your songs are stored. The process will then begin.  
![A screenshot of Nautilus's PS3 Converter. A cursor hovers over "One-Click Batch PS3 Fixer."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3oneclick.png "PS3 Converter")

Any files needing audio encryption or downmixed for PS3 will be updated.

4\. If you want to be sure that the song works in online multiplayer, scroll down to the [[Song ID Tutorial]] below. Otherwise, open Onyx Music Game Toolkit and click `Quick convert/pack`.  
![A screenshot of Onyx's main screen. A cursor hovers over "Quick convert/pack."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3oneclick.png "Onyx Console")

5\. Stay on the `RB quick convert + pack creator` tab. Then click on `Add Rock Band Song` or drag and drop to add the CON files from before.  
![A GIF of customs in CON format being dragged and dropped into the "RB quick convert + pack creator" tab of Onyx.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxdraganddrop.gif "Quick Convert")

It is also recommended to check the box `Author to DTA tag` at the bottom right.  
![A screenshot of Onyx's Quick Convert screen. "Author to DTA" is highlighted and has a cursor over it.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxauthor.png "Quick Convert")

6\. Below the first row of gray buttons, click the first menu and select `Make Packs` or `Make Songs` depending on how you want to combine your songs (packs are recommended).  
![A screenshot of Onyx's Quick Convert screen. "Make songs: produced a single file for each song" has been clicked and the cursor is over "Make packs: combine songs up to a maximum file size."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxmakepackrpcs3.png "Quick Convert")

7\. At the bottom left, make sure `Encrypt .mid.edat` is select, then select between either `PKG (PS3)` or `Folders (PS3)`.  
* `Folders (PS3)` is recommended for RPCS3 users and PS3 users who know how to use FTP. It is **much** faster than PKG creation.
* `PKG (PS3)` is only recommended for PS3 users who can only use USB flash drives to add more songs.

<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a href="#folders" data-toggle="tab">Folders (PS3)</a></li>
    <li><a href="#pkg" data-toggle="tab">PKG (PS3)</a></li>
</ul>
  <div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="folders">
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxoutfolder.png" alt="A screenshot of Onyx's Quick Convert screen. The cursor is selecting &quot;Folders (PS3)&quot; and &quot;Encrypted .mid.edat&quot; has been enabled." title="Quick Convert">
<p>8. <em>(Optional but highly recommended)</em><br>
With these methods, the USRDIR subfolder will have an auto-generated name. For single songs and packs, it’ll be <code>OxxxxxSongName</code>. However, if you make a pack, the folder name will only include the first song in the pack.<br>
If you want to find the folder easily, I recommend selecting <code>Custom USRDIR subfolder</code> instead of <code>Combine into one new USRDIR subfolder per pack</code> and entering the name of your choice.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxfoldernamerpcs3.png" alt="A screenshot of Onyx's Quick Convert screen. The cursor is selecting &quot;Custom USRDIR subfolder&quot; where &quot;Keep original USRDIR subfolders&quot; once was." title="Quick Convert"></p>
<p>You can make a pack with just a single song too. It really helps if you’re trying to locate a song you already installed within the game files.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxnamepack.png" alt="A screenshot of Onyx's USRDIR naming popup. The pack has been named &quot;my_custom_pack.&quot;" title="Quick Convert"></p>
<p>9. At the bottom, select the big button labeled <code>Make pack</code> or (<code>Start</code> if you used the <code>Make Songs</code> option.)<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxmakepackrpcs3.png" alt="A screenshot of Onyx's Quick Convert screen. The cursor is over &quot;Make 1 pack.&quot;" title="Quick Convert"></p>
<p>Navigate to your RPCS3 folder and select the <code>dev_hdd0</code> folder.<br>
If you’re going to be installing to a PS3 via FTP, select the most convenient folder.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/savefolder.png" alt="A screenshot of a file browser window. &quot;dev_hdd0&quot; is selected and the cursor is over &quot;Select folder.&quot;" title="Select Folder"></p>
<p>It should successfully convert and auto-install into your RPCS3 directory, ready to play.<br>
If using RB3DX, you can even do this while the game is running. Within RB3, select:<br>
<code>Options &gt; Extras &gt; Refresh Library</code> to reload your song list.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxcreatedrpcs3.png" alt="A screenshot of Onyx's USRDIR naming popup. The pack has been named &quot;my_custom_pack.&quot;" title="Quick Convert"></p>

</div>

<div role="tabpanel" class="tab-pane" id="pkg">
    <p><img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxoutpkg.png" alt="A screenshot of Onyx's Quick Convert screen. The cursor is selecting &quot;PS3 (PS3)&quot; and &quot;Encrypted .mid.edat&quot; has been enabled." title="Quick Convert"></p>
<p>8. <em>(Optional but highly recommended)</em><br>
With these methods, the USRDIR subfolder will have an auto-generated name. For single songs and packs, it’ll be <code>OxxxxxSongName</code>. However, if you make a pack, the folder name will only include the first song in the pack.<br>
If you want to find the folder easily, I recommend selecting Custom USRDIR subfolder instead of <code>Combine into one new USRDIR subfolder per pack</code> and entering the name of your choice.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxfoldernamepkg.png" alt="A screenshot of Onyx's Quick Convert screen. The cursor is selecting &quot;Custom USRDIR subfolder&quot; where &quot;Keep original USRDIR subfolders&quot; once was." title="Quick Convert"></p>
<p>You can make a pack with just a single song too. It really helps if you’re trying to locate a song you already installed within the game files.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxnamepack.png" alt="A screenshot of Onyx's USRDIR naming popup. The pack has been named &quot;my_custom_pack.&quot;" title="Quick Convert"></p>
<p>9. At the bottom, select the big button labeled <code>Make pack</code> or (<code>Start</code> if you used the <code>Make Songs</code> option.)<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxmakepackpkg.png" alt="A screenshot of Onyx's Quick Convert screen. The cursor is over &quot;Make 1 pack.&quot;" title="Quick Convert"></p>
<p>Select where you would like to save the PKG file and give it a name.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/savepkg.png" alt="A screenshot of a file browser window. The file name has been set to &quot;my_custom_pack&quot;" title="Select Folder"></p>
<p>It should successfully convert and a PKG file will be created, ready to install.<br>
Simply install it like any other PKG.<br>
<img src="https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxcreatedpkg.png" alt="A screenshot of Onyx's USRDIR naming popup. The pack has been named &quot;my_custom_pack.&quot;" title="Quick Convert"></p>

</div>
</div>

## Troubleshooting

### Customs not working online / Scores not saving
The PS3 version of Rock Band 3 can only remember scores for numeric song IDs. If a converted song has letters in the song ID, it will create a new one every time the game starts. This means your score is wiped every time.

Online will also have problems, with songs appearing grey even if you and other players have the same song installed. To avoid this, the CON file needs a numeric ID.

![A screenshot of Rock Band 3, showing songs with a darker color as they are disabled.](https://rb3pc.milohax.org/images/trbl/online/missingsong.png "Rock Band 3: Missing Songs Example")

If you wish to correct the ID of a song you've already installed, click here down to the “Installed Songs section”, otherwise follow the steps below to get a correct ID:

#### Fixing IDs Before Installing

1\. Open Nautilus and select `Batch DTA Processor`.   
![A screenshot of Nautilus. A cursor hovers over "Batch Processor."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilushomebatchproc.png "Nautilus")

2\. Drag and drop any CON in your folder of customs you want to install then click `Begin` to start processing the entire folder.  
**Make sure that `Automatically change alphanumeric songs IDs to unique numeric IDs` is enabled!**  
![A GIF of Nautilus' Batch DTA Processor. Songs are being dragged then dropped into it then, after "Begin" is click, it starts processing.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusbatchfix.gif "Batch DTA Processor")

3\. After it's done, you can go back to step 4 of [[the main tutorial]].

#### Fixing IDs of Installed Songs

1\. Open Nautilus and select `PS3 Converter`.  
![A screenshot of Nautilus. A cursor hovers over "PS3 Converter."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilushomeps3.png "Nautilus")

2\. At the top of the `PS3 Converter` window, go to:  
`Numeric ID Options > Batch replace song IDs`  
![A screenshot of Nautilus's PS3 Converter. A cursor hovers over "Batch replace song IDs" under the "Numeric ID Options" menu.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3batchid.png "PS3 Converter")

3\. On either PS3 or RPCS3, navigate to song/pack containing the song with the bad ID (normally within `dev_hdd0\game\BLUS30463\USRDIR\[SONGNAME]\songs`).  
After finding it, select the `songs.dta` file within the folder. 
![A screenshot of a file browser window. "dev_hdd0" is selected and the cursor is over "Open".](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3batchselect.png "Select DTA file to edit")

4\. Wait for it to finish correcting every song within that pack. When it finishes, you can share the fixed `songs.dta` file with your friends to play the previously unavailable songs together.  
![A screenshot of Nautilus's PS3 Converter. It has just finished replacing custom songs without numeric IDs.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3batchdone.png "PS3 Converter")

## Songs Stuck Looping at the End
Occasionally certain songs may freeze toward the end of the chart, constantly looping the last bits of the audio endlessly.  
* **You will need need the original CON file to fix this issue!**
* **Do not run every song through this if it does not need fixing, the audio will be re-encoded and will have a slight decrease in audio quality**

1\. Open Nautilus and select `PS3 Converter`.  
![A screenshot of Nautilus. A cursor hovers over "PS3 Converter."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilushomeps3.png "Nautilus")

2\. At the top of the `PS3 Converter` window, go to:  
`Tools > Batch fix looping songs`  
![A screenshot of Nautilus's PS3 Converter. A cursor hovers over "Batch fix looping songs" under the "Tools" menu.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3batchloop.png "PS3 Converter")

3\. Go to the folder where the problematic CON is at and select the folder.  
Wait for it to finish.
![A screenshot of Nautilus's PS3 Converter. It is in the process of fixing a looping file.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3batchloopproc.png "PS3 Converter")

4\. After it's done, you can go back to step 4 of [[the main tutorial]].

## Delete individual songs in a pack

Rock Band 3 can delete a song in-game. The problem is, if a song is part of a pack, it'll delete that entire pack as well.  
![A screenshot from Rock Band 3, warning the user that they're about to delete many songs from the library.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/rb3delwarn.png "Delete song")

The best way to remove a song from a pack is through Nautilus' "Quick Patch Editor."

1\. Open Nautilus and select `Quick Pack Editor`.  
![A screenshot of Nautilus. A cursor hovers over "Quick Pack Editor."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilushomepack.png "Nautilus")

2\. Open a file browser window and navigate to the pack folder that contains the song you want to remove and look for the `songs.dta` file.  
It will usually be in `dev_hdd0\game\BLUS30463\USRDIR\[PACKNAME]\songs`).
![A screenshot of a file browser window. "songs.dta" is selected.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/findfolder.png "songs")

3\. Drag the `songs.dta` file into the `Quick Pack Editor`.  
Select the songs you want to remove then click `Remove selected`.  
When you're done, click `Save` to lock your changes in.  
![A GIF of a "songs.dta" file being dragged and dropped into Nautilus' Quick Pack Editor.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautiluspackdrag.gif "Quick Pack Editor")

4.\. Even though the song is deleted from the `songs.dta` file, they will still take up space.  
You have to delete the song's corresponding folder as well.  
![A screenshot of a file browser window. Multiple songs are selected and the cursor hovers over a popup menu option that says "Delete."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/packdelfolder.png "songs")

## PS3: Greyed out customs

By default, the PlayStation 3's Parental Controls are set to level 9.  
This doesn't allow customs that are classified as "Unrated", causing them to appear grey. 
![A screenshot of Rock Band 3's song library. It shows as greyed out song.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/ps3grey.png "Rock Band 3: Grey Songs")

Selecting these songs will cause a crash.
To fix this, set the `Parental Control` to `Off` in:  
XMB: [ **Settings** ] -> [ **Security Settings** ] -> [ **Parental Control** ] -> [ **Off** ]  
![A screenshot of the parental control menu in PlayStation 3's XMB home menu. The level is set to "Off".](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/ps3parental.png "Parental Control")

## Songs still infinite loading

In very rare cases, songs might still have infinite loading, even after the using PS3 fixer.  

Do note that you'll need to have "Rock Band 3 1.1 Beta 4" or newer if you're on PS3.  

1\. Open Nautilus and select `Batch Cryptor`.  
![A screenshot of Nautilus. A cursor hovers over "Batch Cryptor."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilushomepack.png "Nautilus")

2\. Swap to `Decrypt` at the bottom of the screen.  
![A screenshot of Batch Cryptor. The mode has been switched to "Decrypt."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautiluscryptdecrypt.png "Batch Cryptor")

3\. On either PS3 or RPCS3, navigate to the folder containing the song you wish to fix.  
It will usually be in `dev_hdd0\game\BLUS30463\USRDIR\[PACKNAME]\songs\[PROBLEMATICSONG]`).  
There will be a `.mogg` file in the song's folder.  
![A screenshot of a file browser window. A mogg file is selected.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/findmogg.png "MOGG File")

4\. Drag and drop the song's `.mogg` file onto `Batch Cryptor` and click `Begin`.  
![A GIF of a .mogg file being dropped into "Batch Cryptor" the being decrypted.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautiluscryptdecryptmogg.gif "Quick Convert")

5\. A new folder called `decrypted` will appear when it finishes.  
Go into the new `decrypted` folder and cut the `.mogg` file inside of it.  
Go back to the song's main folder and replace the old `.mogg` file.
![A GIF of a .mogg file within the "decrypted" folder being cut then pasted in the folder before it. It replaces the old .mogg file.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/moggreplace.gif "Quick Convert")

## Converting Clone Hero/YARG songs to Rock Band 3

<span style="font-size:xxx-large;">DISCLAIMER - READ BEFORE CONTINUING</span>

Do this as a **last resort** if the charts you want to convert were specifically made for PC clone games (Clone Hero/YARG). If the chart originally existed in RB format, whether it be official DLC or customs, **get that first and follow the main guide at the top!**

**Failure to do so will result in lost metadata** associated with the original song package, including:
* Incompatibility with any song upgrades in RB3DX
	* Keys, Pro Guitar, Harmonies, & chart fixes to legacy RB songs that didn't have them
* Incompatibility with online play and leaderboards
* Animation data such as character lipsync will be lost

Should you decide to ignore the disclaimer and proceed, you will be **refused any support** from the MiloHax Discord if you run into any issues.
**YOU HAVE BEEN WARNED!**

1\. After downloading the charts you want, open Onyx and select `Batch recompile`.  
![A screenshot of Onyx's main screen. A cursor hovers over "Quick convert/pack."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/nautilusps3oneclick.png "Onyx Console")


{% include links.html %}