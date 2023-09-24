# Creating action sets in controller templates

## Story:
In a previous article we talked about using the native steam deck controller settings to flip the behavior of our left/right joysticks for the N64 game Perfect Dark, specifically.
However, two things to note by following that guide:
1. The change is a global change, effecting everything that uses said template.
   - In this example, I use emulation station to launch all my emulator games.  If I edit the emulation station game controller config to flip the joysticks, then this change applies to EVERY game, not just perfect dark
   - This is not ideal as almost all other games work just fine using the default configuration, so this change would ultimately end up BREAKING more games than fixing, which we dont want
2. Since this is a global change, it is not specific to N64 at all.  This means, any future games we execute from Emulation Station that may have the same issue, we can apply the exact same fix adhoc

Since we are using Emulation Station as our "Emulation Hub", what we are going to do is create what is called a "Action Set" for the Emulation station game controller settings
- This action set will be called "Flip Joysticks"
- The function of this action set will be to apply the Left/Right behavior when selected
- The behavior will revert back to normal controls when action set is not enabled

## Step 1: Creating the action set
1. Select Emulation Station -> Click "Controller" icon to edit controller settings -> click "Edit Settings"
2. Scroll down to bottom on left side column and highlight "Action Sets"
3. Scroll down to bottom on right side column and select "Create new"
4. Select the "Emudeck Hotkeys" as the template.  This will allow the button mapping configuration to apply the same as the default emudeck config
5. Proceed to follow the steps in <link flipjoysticks.md> to make changes to joystick behavior
6. Press "B" button on gamepad to go back to main controller settings screen

## Step 2: Creating a Menu
Now that the action set for flipped joystick behavior has been created, how do we use it?
Great question, with a detailed answer: When you use Emulation station, have you noticed when you brush your thumb over the left trackpad, a little menu pops up?

- We will be leveraging that existing menu by creating a new sub menu then adding that sub menu to the main menu.  
- The expected result is when we launch emulation station, and select a game that requires the flipping of the joysticks, we can pull up the menu, enable the joystick flip, and game on
- When finished, either exiting emulation station will reset the controls back to normal, or we can reset the controls manually via the menu

1. Missing steps.. need to re-create and document
2. See above.


## Testing the new action set:

1. Open emulation station -> select game that requires joystick behavior flip (I.E. Perfect Dark N64)
2. using the emulation station menu (default triggered via the left touchpad) select your "Joystick Flip" menu/action set
3. Default behavior will enable the flip by default, so effects should be implemented immediately for testing
4. Confirm behavior matches expectations.  Enjoy the game a little!
5. To test reverting back to defaults, from the action set menu -> Select "Go back to previous menu"
6. This will revert joystick behavior back to default Emulation Station configuration
7. Open another game and confirm stock joystick behavior is present

Conclusion:
This is a neat feature which will enable quick customizations on the fly while in game.
What are your use cases for action sets/menus?  We'd love to hear some of your examples!



