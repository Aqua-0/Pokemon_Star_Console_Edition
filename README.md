# Pokemon Star v0.2: Console Edition


Taking Pokemon Star v0.2, made by Rusyaas and turning it into a console-playable state.
WARNING: If you have already downloaded Pokemon Ultra Moon (not using a cart), make (ABSOL)UTELY SURE that you do ALL the instructions later on. Without, bad things may happen...

# Prerequisites #

A homebrewed 3DS on the latest version of Luma3DS with boot9strap (If you haven't homebrewed your 3DS yet, follow 3ds.guide to join the party.)
Your 3DS SD Card must have at least 8GB of space.
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
5. Scroll down the list until you see Pok??mon Ultra Moon. (Number to left ends in 001B5100!)
6. Select "TMD file options..."
7. Select "Build CIA (standard)" (This will take some time.)
8. Turn off the 3DS, then copy the CIA you built to the PC.
9. Use https://github.com/davFaithid/CIA-to-3DS-Rom-Converter/releases to convert the CIA to a 3DS ROM. (Instructions should be in the two batchfile zip.)
10. Move the ROM back to the 3DS.

## Rip a .3ds rom from cartridge (Also Recommended) ##
1. Boot into GodMode9 by holding Start upon boot. If you see multiple options, select GodMode9.
2. Insert your cart, then find 00040000001B5100_v00.3ds in [C:] GAMECART.
3. Push A, then select NCSD image options, then choose Decrypt file (0:/gm9/out) (This will take some time.)

## Download a .3ds rom (Unrecommended, unless you have Ultra Sun) ##
1. Find the .3ds rom somewhere and move it to your 3DS. (Blatant piracy isn't cool, so I can't help you with this one. Downloading it will take some time, depending on your internet speed.)


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
9. Go into content0.game, but this time copy the entire romfs and exefs folders, in addition to extheader.bin to somewhere on your SD card.
10. Replace the content0.game/romfs/a/0/8/3 file with the one you got from the UM rom.
11. Turn off your 3DS, then put the spliced together romfs folder and the untouched exefs folder back onto your computer.
12. In the folder where you installed HackingToolkit9DS, there should be an ExtraTools folder (For convinence sake, put the folders there.
13. Replace the banner and icon files in the exefs folder from the ones I posted on the Github, and rename the file .code file to .code.bin. (Weird things happen if you don't.)
14. Run the tool 3DS Builder Mod.
15. Select the romfs folder that you spliced together, the exefs folder, and the extheader.bin file. (If you know what you're doing, modify them to your liking. But I don't, so we won't touch that.)
16. Put in a serial number. Put anything down that isn't already in use! (CTR-P-STAR works just fine.)
17. Wait for it to build, then move it to your 3DS. 
18. Select "NCSD image options", then choose "Build CIA from file", then pray to your deity of choice that it works. (This will take some time. If there's an error, make sure that you didn't forget any steps. (If you see an ETA, it's a good sign!)
19. If you play Ultra Moon downloaded from the eShop, proceed with the rest of Creating The Rom. Otherwise, just skip it.
20. Turn off your 3DS, the


# Cleanup #
1. If you picked the correct deity, or got super lucky, then this went of without a hitch! (Can't say the same for me writing this...) As Gamechamp3000 said in her first video about a low-shot run of Octo Expansion, "Turns out all you needed to conquer death was a spoonful of elbow grease and a freighter loaded with pain and suffering!"
2. Delete the original .3ds file and the downloaded pokemon star .3ds file if you haven't already.
3. Reboot your 3DS, then install the file with FBI.
4. Fire up the game. If you see Kukui instead of Wicke, you messed up somewhere. The text from anytime after the opening cinematic should be the same, but the models will still be the originals. :(
5. Delete the spliced together pokemon star .3ds file.
6. Delete the applications you had to install as a part of the setup.


# Migrating from Citra #
1. Boot the spliced together game on your 3DS at least once.
2. Select your Pokemon Star save file from Citra, then copy it over. (I'll go more into detail when I finish this guide...)


# Changelog & Things To Note #
Until mentioned otherwise, the overworld will remain the same. My apologies, it's just a limitation of that imfamous a083 garc. Maybe it'll be fixable in the future?
v0.1: First sucessful experiment.
Banner and icons: Replaceable.
Modded a083 garc: Probably still broken.
Thinking about trying to fix a083 garc: Some day...
