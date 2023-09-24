# Flipping the behavior of the left and right joysticks if needed

## Story:
Recently I tested playing some N64 games in EmuDeck, including Goldeneye and Perfect Dark.  The default controls worked well enough in Goldeneye, despite the awkwardness for its generation, it was completely playable.
Perfect dark, however, I could not get a controller config that felt normal in my hands, leaving the game largely unplayable.  The closest I came was changing the in-game controller settings, which mapped:
  - aiming set to the left joystick (head bob up, down, aim left/right).
  - moving set to the right joystick (Forward, back, strafe left/right).

To anyone accoustomed to controller gaming, you might notice the behavior of these two joysticks are, in a word, flipped around.  I prefer that strafing/moving be done with the left joystick, with the aiming done on the right.
So how can we resolve this and get into the action?

## The quickest solution to this issue:
To quickly resolve the issue, Steam Deck controller settings provides us with the solution: 
1. Open emudeck -> click controller icon -> edit controller
2. Scroll down to "Joysticks" on the left hand column
3. Under "Joysticks" settings -> locate where it says "Left Joystick Behavior" -> ensure "Joystick" is the select output -> Click the "Gear" icon next to the word "Joystick"
  <Insertscreenshothere>
5.Scroll down to "Output" -> highlight "Output Joystick" setting -> Select "Right joystick" and from the resulting dropdown box select "Left Joystick" to change
6. Press "B" button to go back to the previous screen
7. Locate the "Click" setting -> press "Right Click Stick" to open the input select screen
8. Ensure the "GamePad" tab is open -> highlight the "L" stick in the upper left hand corner -> press "A" to select the left stick click button

This will swap the behavior of the right joystick to function as the left joystick.  
- Repeat the steps above for the left joystick behavior, swapping references to "left" with "right"

Once finished with both joysticks, test in game by confirming the behaviors of the left/right joysticks are now "flipped back" and functioning as expected

## Conclusion:
This is a great little trick to quickly swap your inputs without having to modify any emulator specific settings.  Using Steam Deck controller settings makes it so that 
1. The changes can be saved as a template for later use
2. The changes can be easily reverted via the steam overlay menu
3. We can expand further with Action Sets, Menus and other features using the Steam Deck Controller settings vs emulation or in-game settings <link to article about action sets>
