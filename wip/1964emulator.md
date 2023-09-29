# What is the 1964 emulator and why should I install it?

## Story:
One of my most looked forward to tests on the steam deck was enabling wasd+mouse for first person shooters of my favorite console games.  Like some gamers, I find 
myself better at certain generes on PC due to the flexibility and precision of the keyboard and mouse combo.  Racing games are not one of those generes!

Some of those games include:
- N64 classics Goldeneye 007 and Perfect Dark
- Timesplitters and Black on Xbox/PS2
- Metroid Prime on GameCube/Wii

In the instance of Metroid Prime, we get the wonderful Prime specific emulator which can also be installed as part of the EmuDeck package, and is highly recommended
to do so at the time of installation.  We will circle back on Timesplitters and other FPS's on other consoles in another article.

That leaves our beloved N64 classics Goldeneye and Perfect Dark.  Sure, we could configure the touchpads to mimick joystick control, however we are still left with
an experience that doesnt feel all that different from the original outing.  What if Goldeneye actually felt like it was made for PC?

## Enter 1964
This brings us to the 1964 emulator.  Funky name, amazing emulator.  It is a custom made package made from a combination of sources required to recreate the look and
feel of the games.  
- wasd+mouse plugin
- high res textures
- specific version of n64 emulator
- custom configured settings for steamdeck

That last point is rather interesting, as there is a specific fork of the emulator specificall for us steam deck users.  Pretty cool.

## Installation Steps (Step 1):
Installation is as simple as it can get.  
1. On your deck switch to desktop mode
2. Open web browser and browse to https://github.com/Graslu/1964GEPD/releases
3. Scroll down until you see the 1964 for Steam Deck build
4. Click the filename to begin downloading the emulator
5.Browse to the location downloaded -> open zip file
6. If Emudeck is already installed, browse to Emulation -> Storage
   - Create a new folder named "1964"
7. Extract the emulator contents into the "1964" folder

Success!  The 1964 emulator is now technically installed. While the emulator can be used in typical fashion, i.e. open the emulator, select your game, play game,
however we will next be configuring games so that they can be added with game art and launched via Game Mode

## Adding Goldeneye 007 (Step 2A)
- Note: A Goldeneye v1 US .n64 or .z64 rom is required. We do not advocate piracy and are unable to assist with roms. If unsure of compatability, follow steps to add your rom file and open 1964 emulator.  There will be a note 
indicating compatability, if incompatible version is used mouse will not function.
1. Make a copy of your Goldeneye 007 rom and paste it in the root "1964" folder created during the installation steps
2. Rename your file to `ge`, all lowercase
3. Open desktop Steam client -> Library
4. Click "Add non-Steam game"
5. Browse to location of "1964" emulator
6. Select "1964.exe" -> add to Steam
7. Edit "1964.exe" game properties
8. Rename "1964.exe" -> "Goldeneye - 007".  If spelled exactly, controller template will appear under "Controller" settings
9. Testing -> Launch game from Steam Client, verify mouse controls are working via the touchpad.  Play the game a little!

## Adding Perfect Dark (Step 2B)
- Note: A Perfect Dark v1.1 US .n64 or .z64 rom is required. We do not advocate piracy and are unable to assist with roms. If unsure of compatability, follow steps to add your rom file and open 1964 emulator.  There will be a note 
indicating compatability, if incompatible version is used mouse will not function.
- Note 2: Steps can be done in tandem with Goldeneye
1. Make a copy of your Perfect Dark rom and paste it in the root "1964" folder created during the installation steps
2. Rename your file to `pd`, all lowercase
3. Open desktop Steam client -> Library
4. Click "Add non-Steam game"
5. Browse to location of "1964" emulator
6. Select "1964.exe" -> add to Steam
7. Edit "1964.exe" game properties
8. Rename "1964.exe" -> "Perfect Dark".  If spelled exactly, controller template will appear under "Controller" settings
9. Testing -> Launch game from Steam Client, verify mouse controls are working via the touchpad.  Play the game a little!

