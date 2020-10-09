# Pokemon Star v0.2: Luma Edition
Taking Pokemon Star v0.2, made by Rusyaas and turning it into a Luma3DS patch that may be console-playable.

Disclaimer: This is very experimental, and very unfinished. If you want to help this to not be a lost cause and finally make Pokemon Star playable on console, throw all the ideas you have at me.

# Prerequisites #

A homebrewed 3DS on the latest version of Luma3DS with boot9strap (If you haven't homebrewed your 3DS yet, follow 3ds.guide to join the party.)

3DS SD Card with at least 8GB of free space (Assuming that you have not installed Ultra Moon or downloaded the rom hack)

A computer that can access your SD card (You're probably reading this readme on that computer.)


# Installing Ultra Moon #

Get some form of Pokemon Ultra Moon. Download and install a rom from that site, grab your cart, rip then install a rom, just get Ultra Moon on your 3DS in a playable state somehow. However, I highly recommend supporting the devs and downloading Ultra Moon off of the eShop or buying an Ultra Moon cart if you don't have it or Ultra Sun. :D Those methods are much quicker and simpler, and they tell Game Freak that you like USUM, and hope they do more games like that in the future.
(Note that only Ultra Moon will work for these instructions. The rom hack simply wasn't made with Ultra Sun in mind.)



## eShop Method (Recommended) ##
1. Download the game off the eShop.
2. You're done!


## Using a regular cart (Recommended) ##
1. No setup needed! Go to Installing The Rom Hack! :D (Note that you will need to insert your Ultra Moon cart every time you want to play Pokemon Star, and for the rest of the guide we'll assume that you have your cartrige inserted.)


## Convert .3ds rom to CIA ##
1. Do one of the two below methods for getting your rom.
2. Select NCSD image options, then choose Build CIA from file. (This will take some time.)
3. Use FBI to install the CIA. (This will take some time.)


### Rip a .3ds rom from cartridge ###
1. Boot into GodMode9 by holding Start upon boot. If you see multiple options, select GodMode9.
2. Insert your cart, then find 00040000001B5100_v00.3ds.
3. Push A, then select NCSD image options, then choose Decrypt file (0:/gm9/out) (This will take some time.)
4. Go to gm9/out in the SD card drive, then select NCSD image options, then choose Trim file.
5. Go on to Convert .3ds rom to CIA.

### Download a .3ds rom (Unrecommended) ###
1. Find the .3ds rom somewhere. (Blatant piracy isn't cool, so I can't help you with this one.)
2. If the rom is 4gb, then trim it using a program like NDSTokyoTrim (https://eden.fm/ndstoykotrim/).
3. Go on to Convert .3ds rom to CIA.


## Install a CIA from the internet (Very unrecommended) ##
1. Find the .cia somewhere. (Blatant piracy isn't cool, so I can't help you with this one. Be careful, tainted CIAs may do something malicous or be the wrong game)
2. Use FBI to install the CIA. (This will take some time.)



# Installing The Rom Hack #

If migrating from Citra, go to Migrating From Citra.
1. If applicable make a backup of your Ultra Moon save using Checkpoint (you should already have it), name it something you'll remember (like UltraMoonSave), then delete your savefile in-game with D-Up + X + B. (Don't delete the backup!) Shut down your 3DS afterwards.
2. Download PokemonStarLuma.zip (Very large, so will likely take a while.)
3. When you've downloaded it, unzip it and move the romfs folder inside to /luma/titles/00040000001B5100 on your 3DS's SD card. (If the folder doesn't exist, create it)
4. Hold Select when turning your 3DS back on.
5. Turn on game patching in the Luma3DS config menu, then press start to leave the menu.
6. Open Pokemon Ultra Moon and watch the fireworks fly. If you get a green screen, then the top of the screen says Pokemon Star v0.2 after the title screen, it's a good sign.


## Migrating from Citra ##
1. Boot vanilla Ultra Sun on your 3DS at least once.
2. Select your Pokemon Star save file from Citra, then copy it over 


# Going Back To Vanilla #

1. Go into Checkpoint and make another save backup. Name it something you'll remember, like PokemonStarSave.
2. Restore your vanilla save backup.
3. Turn off your 3DS, then turn it on again while holding Select.
4. Turn off game patching in the Luma3DS config menu, then press start to leave the menu.
5. If you want to delete Pokemon Star, then go into /luma/titles/00040000001B5100 and delete the romfs folder. (Optional)


# Going Back To Pokemon Star #

1. Follow Going Back To Vanilla, but do the opposite of 1 - 4. (Back up your vanilla save, restore your Pokemon Star save, then turn back on game patching.)
2. If you deleted Pokemon Star, redownload it and put it back in /luma/titles/00040000001B5100.


# Changelog #
v0.1: Initial Release (3.51 GB Install Size)
The original release of Luma Edition. Probably won't work.
