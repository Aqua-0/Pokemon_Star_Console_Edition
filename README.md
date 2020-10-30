# Pokemon Star v0.2: Console Edition
# Note: This guide is currently undergoing renovations! #
RadoMiami was updating this guide, but then he got sleepy and decided to go to bed. In the meantime, please ignore the below instructions.


Taking Pokemon Star v0.2, made by Rusyaas and turning it into a console-playable state.
WARNING: If you have already downloaded Pokemon Ultra Moon, make (ABSOL)UTELY SURE that you have changed the Title ID of the final rom you'll have. Otherwise, you may find that either your Pokemon Star spliced together ROM won't install or your vanilla Ultra Moon suddenly dissapears after installing. (The guide does NOT go over this, so you're unfortunately in the woods for now.) Furthermore, this WILL take a long time. Be prepared to bring your breakfast and lunch to your computer desk.

# Prerequisites #

A homebrewed 3DS on the latest version of Luma3DS with boot9strap (If you haven't homebrewed your 3DS yet, follow 3ds.guide to join the party.)
Your 3DS SD Card must have at least 4GB of space.
Your PC must have at least 12GB of space. (The rom hack won't take all this space for long, it will be reclaimed soon afterwards.)
A computer that can access your SD card (You're probably reading this readme on that computer.)
Basic knowledge on how to use GodMode9, Checkpoint, and HackingToolkit9DS. (You should have the first two, the third is at https://github.com/Asia81/HackingToolkit9DS-Deprecated-/releases).


# Obtain An Ultra Moon ROM #

Get some form of a Pokemon Ultra Moon ROM. Download and install a rom from that site, rip a rom, just get the Ultra Moon ROM somehow. However, I highly recommend supporting the devs and downloading Ultra Moon off of the eShop or buying an Ultra Moon cart if you don't have it or Ultra Sun. :D Those methods tell Game Freak that you like USUM, and hope they do more games like that in the future.
(Note that only Ultra Moon will work for these instructions. The rom hack simply wasn't made with Ultra Sun in mind.)

## eShop Method (Recommended) ##
1. Download the game off the eShop. (In this instance, make sure you have 8GB of free space before continuing!)
2. Boot into GodMode9.
3. Go into [A:] SYSNAND SD, then /title/.
4. Press R+A while highlighting the 00040000 folder, then select "Search for titles".
5. Scroll down the list until you see Pokemon Ultra Moon. (Ends in 001B5100!)
6. Select "TMD file options..."
7. Select "Build CIA (standard)" (This will take some time.)

## Rip a .3ds rom from cartridge (Also Recommended) ##
1. Boot into GodMode9 by holding Start upon boot. If you see multiple options, select GodMode9.
2. Insert your cart, then find 00040000001B5100_v00.3ds in [C:] GAMECART.
3. Push A, then select NCSD image options, then choose Decrypt file (0:/gm9/out) (This will take some time.)

## Download a .3ds rom (Unrecommended) ##
1. Find the .3ds rom somewhere. (Blatant piracy isn't cool, so I can't help you with this one. Downloading it will take some time, depending on your internet speed.)


# While You Wait... #
While you're waiting to get your UM rom, download Pokemon Star from that site. (If you already have it, skip this.) (Search "pokemon star rom", and you'll eventually find what you need.) Both will take a while, so it's better to knock them both out now.


# Creating The Rom #
1. After downloading HackingToolkit9DS, put the .3ds Pokemon Star rom in the PackHack folder.
2. Make sure you run SetupUS.exe first, or it may not work.
3. After it finishes, trim your Pokemon Star rom on your PC using something like NDSTokyoTrim.
4. Mount the ripped Ultra Moon rom by selecting NCSD image options, then Mount image to drive.
5. Go into content0.game/romfs/a/0/8, then copy the file called "3" to some place on your SD card. If you want, rename it to something like "clean a083", though note you will have to change its name back later.
6. Select the Ultra Moon rom again, then push A when it tells you to unmount to unlock the file.
7. If you're not planning on converting it into a CIA, delete the Pokemon Moon rom, then turn off the 3DS.
8. Put the trimmed Pokemon Star rom on your 3DS, then do 7 again with it.
9. Go into content0.game, but this time copy the entire romfs and exefs folder to somewhere on your SD card.
10. Replace the content0.game/romfs/a/0/8/3 file with the one you got from the UM rom.
11. Turn off your 3DS, then put the spliced together romfs folder and the untouched exefs folder back onto your computer.
12. In the folder where you installed HackingToolkit9DS, there should be an ExtraTools folder.
13. Run the tool 3DS Builder Mod.
14. Select the romfs folder that you spliced together, the DecryptedExeFS.bin file from the main folder, and the DecryptedExHeader.bin file from the main folder. (If you know what you're doing, modify them to your liking. But I don't, so we won't touch that.)
15. Put in a serial number. Put anything down that isn't already in use! (CTR-P-STAR works just fine.)
16. Wait for it to build, then move it to your 3DS. 


# Cleanup #
1. If you picked the correct deity, or got super lucky, then this went of without a hitch! (Can't say the same for me writing this...) As Gamechamp3000 said in her first video about a low-shot run of Octo Expansion, "Turns out all you needed to conquer death was a spoonful of elbow grease and a freighter loaded with pain and suffering!"
2. 

# Migrating from Citra #
1. Boot the spliced together on your 3DS at least once.
2. Select your Pokemon Star save file from Citra, then copy it over. (I'll go more into detail later...)


# Going Back To Vanilla #

1. Go into Checkpoint and make another save backup. Name it something you'll remember, like PokemonStarSave.
2. Restore your vanilla save backup.
3. Turn off your 3DS, then turn it on again while holding Select.
4. Turn off game patching in the Luma3DS config menu, then press start to leave the menu.
5. If you want to delete Pokemon Star, then go into /luma/titles/00040000001B5100 and delete the romfs folder. (Optional)


# Going Back To Pokemon Star #

1. Follow Going Back To Vanilla, but do the opposite of 1 - 4. (Back up your vanilla save, restore your Pokemon Star save, then turn back on game patching.)
2. If you deleted Pokemon Star, redownload it and put it back in /luma/titles/00040000001B5100.


# Changelog & Things To Note#
Until mentioned otherwise, the overworld will remain the same. My apologies, it's just a limitation of that imfamous a083 garc. Maybe it'll be fixable in the future?

v0.1 Initial Release (??? GB)
Trying to find out a way that it'll work... Hang tight!
