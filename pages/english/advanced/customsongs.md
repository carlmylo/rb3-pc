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

<span style="font-size:larger;">This guide is primarily focused on customs songs, do not attempt to run official RB content through the fixer.</span>

The main guide on page 2 will fix two major problems the PS3 has with customs that the 360 doesn’t and should follow for every custom you add.
* Infinite loading from improper encryption
* Crash from too high-quality audio

### Requirements:
* A modded PS3 console (with a method of transferring files to it) or the [[RPCS3 emulator]](https://rpcs3.net/){:target="_blank"}
* [[An installation of Rock Band 3 Deluxe]](https://rb3dx.milohax.org/){:target="_blank"} (Optional but highly recommended)
* [[Nautilus version 4.8.4 or later]](https://nemosnautilus.com/nautilus/){:target="_blank"} (Previously known as C3 CON Tools/C3Tools)
	* [[Mirror Link]](https://github.com/trojannemo/Nautilus/releases/){:target="_blank"}
* [[Onyx Music Game Toolkit]](https://github.com/mtolly/onyxite-customs){:target="_blank"}

## Converting to Xbox 360 CONs to PS3
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
![A screenshot of Onyx's Quick Convert screen. "Make songs: produced a single file for each song" has been clicked and the cursor is over "Make packs: combine songs up to a maximum file size."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxmakepack.png "Quick Convert")

7\. At the bottom left, make sure `Encrypt .mid.edat` is select, then:

select `Folders (PS3)``.  
This is recommended for RPCS3 users and PS3 users that know how to use FTP.  
![A screenshot of Onyx's Quick Convert screen. The cursor is selecting "Folders (PS3)" and "Encrypted .mid.edat" has been enabled.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxoutmakerpcs3.png "Quick Convert")

8\. _(Optional but highly recommended)_
With these methods, the USRDIR subfolder will have an auto-generated name. For single songs and packs, it’ll be `OxxxxxSongName`. However, if you make a pack, the folder name will only include the first song in the pack.  
If you want to find the folder easily, I recommend selecting Custom USRDIR subfolder instead of `Combine into one new USRDIR subfolder per pack` and entering the name of your choice.  
![A screenshot of Onyx's Quick Convert screen. The cursor is selecting "Custom USRDIR subfolder" where "Keep original USRDIR subfolders" once was.](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxfoldernamepkg.png "Quick Convert")

You can make a pack with just a single song too. It really helps if you're trying to locate a song you already installed within the game files.  
![A screenshot of Onyx's USRDIR naming popup. The pack has been named "my_custom_pack."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxnamepack.png "Quick Convert")

9\. At the bottom, select the big button labeled `Make pack` or (`Start` if you used the `Make Songs` option.)  
![A screenshot of Onyx's Quick Convert screen. The cursor is over "Make 1 pack."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxmakepackrpcs3.png "Quick Convert")

Navigate to your RPCS3 folder and select the `dev_hdd0` folder.  
If you're going to be installing to a PS3 via FTP, select the most convenient folder.  
![A screenshot of a file browser window. "dev_hdd0" is selected and the cursor is over "Select folder."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/savefolder.png "Select Folder")

It should successfully convert and auto-install into your RPCS3 directory, ready to play.  
If using RB3DX, you can even do this while the game is running. Within RB3, select Options > Extras > Refresh Library to reload your song list.  
![A screenshot of Onyx's USRDIR naming popup. The pack has been named "my_custom_pack."](https://raw.githubusercontent.com/carlmylo/rb3-pc/refs/heads/main/images/xtra/customs/onyxcreatedrpcs3.png "Quick Convert")



{% include links.html %}