# ducky-one-2-mini-mac
Back up for fixing ducky one 2 mini on Mac since reddit is a volitile information source...

Reference: https://www.reddit.com/r/MechanicalKeyboards/comments/e38n17/ducky_one_2_mini_and_mac_os/

Terrible-Possibility:
> Possible Solution - Hope this helps someone out

> Issue: Keyboard randomly stops functioning (no key presses detected), one row of lights stays on - Unplugging and Replugging the keyboard back in, temporarily resolves the problem

> Fix: Override the Ducky USB Vendor ID and Product ID so OSX thinks its a Mac Keyboard

> Hold Fn + Alt + P for 3 seconds
0-9 & A-F will light up (Hexadecimal Input)
Type 05AC024F (This is an Apple Vendor & Product ID)
Unplug and Replug the keyboard
If you want to confirm the change has worked, Open up the System Report, and Look at the Ducky One2 Mini under USB, you should see Product ID: 0x024f & Vendor ID: 0x05ac

maggu01:
> It seems that 024F references the ANSI version of the Apple Magic Keyboard. This caused some bugs for me, since I have ISO layout on my keyboard.

> Solution that seems to be working for me: Replace step 3 with "05AC0250" if you have ISO layout. (Product ID: 0x0250 and same Vendor ID)

[deleted]
> I have a mecha mini. They changed the vendor ID overrides can only be applied with dip 3 on. I tried doing this and now the keyboard won’t turn on when plugged into a macbook.

Turning on DIP 3 worked for me ^^
