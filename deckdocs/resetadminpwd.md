# How to reset your Admin password if lost or forgotton

# Story:
In a previous article, we showed you how to set your admin password and advised to document it in the event that its lost or forgotton over time.  Fret not,
as we can and are indeed able to reset the password with a little bit of work should it be needed.

# Pre-requisites:
1. Steam Recovery OS on bootable USB
2. Dedicated Keyboard and Mouse
3. USB-C to USB-A hub for all the devices above

# Steps:
1. Boot into recovery usb
2. open terminal from desktop, should be fourth icon
3. Type `passwd deck`, type your new password, document it
   - This is the password for the Recovery Environment.  This does not set the new password for the main
5. Type `sudo ~/tools/repair_device.sh chroot`
6. Type `steamos-readonly disable`
7. Open Dolphin file browser
8. Navigate around until it asks to mount a partition, which should be the deck partition (I knew it was mine since the emudeck folder was in home)
9. Right click on an empty space in dolphin -> Click "Terminal"
10. Type `cd ..` until the current directory becomes "tmp-(string of characters)" that has etc, root etc.
11. Type `sudo chroot .`
12. Type `cd etc`
13. Type `mount -o remount /`
14. Type `nano shadow`
15. Find the deck entry
16. Delete everything between first and second colon
17. Press "ctrl+x" -> "y" on keyboard to save
18. Type `nano passwd`
19. Delete the "x" in deck's entry
20. Press "ctrl+x" -> "y" on keyboard to save
21. Type `exit`, several times until "Terminal" window closes entirely
22. Restart Steam Deck
23. Switch to Desktop mode
24. Open Start menu -> Terminal
25. Type `passwd deck`, Type set new password
26. Proceed to Testing steps

# Testing Steps:
Sudo should now be working again with the new password.  To test:
1. Execute an application that prompts for admin password
2. Type the new password and confirm application executes as expected

# Note:
These steps were found and tested from the following Reddit thread.  All credit goes to the OP for providing their findings, we are posting for further visibility

# References:
https://www.reddit.com/r/SteamDeck/comments/uvhe9r/forgot_desktop_mode_user_password_how_do_i_fix/
