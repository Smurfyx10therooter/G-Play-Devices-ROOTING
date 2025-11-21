# G-Play-Devices-ROOTING
How to root the phones like Moto G Play 202+
Tutorial:

Part 1: Setting up

1. Find this website (https://en-us.support.motorola.com/app/standalone/bootloader/unlock-your-device-b)
Sign in with Google or other account
Keep it open for later
--USING TOOLS--
You will need platform tools, so go to (https://developer.android.com/tools/releases/platform-tools) to get the right tools.
Download the tools for your PC. (Windows)
To use the tools, go to your file explorer and extract the zip you just downloaded.
Go into the platform-tools-latest-XxX folder you just downloaded, and find the platform-tools folder inside.
You will see a bunch of .exes (or other file names if you are using Mac/Linux)
To get the tools working, you will need a Terminal. The Terminal is built into your system, so we need to launch the Terminal, follow this.
For Windows
Find the top bar in the file explorer that you found the platform-tools folder inside of the platform-tools-latest-XxX folder.
It should say something similar to "Downloads > platform-tools-latest-XxX > platform-tools" (or downloads might be different depending on where you put your downloaded platform-tools-latest-XxX.zip)
If you find the top bar, click the bar and type in "cmd" all lowercase.
A black hacker-terminal looking window will pop up. Type adb version into the window. If it says something similar to "Android Debug Bridge version X.x.Xx Version xX.x.x-XxXxXxX
Installed as C:\Users\You\Folder\platform-tools-latest-XxX\platform-tools\adb.exe
Running on Windows Xx.X.XxXxX"
If it says that, keep the window open for later as the tools are working.

Part 2: Bootloader Unlocking

Go back to the (https://en-us.support.motorola.com/app/standalone/bootloader/unlock-your-device-b) that you saved for later

Install the Moto USB drivers (https://en-us.support.motorola.com/app/usb-drivers) for Windows

Follow the tutorial until you see "Next, you will need to get your device ID."

The Terminal/CMD window you opened, will be put at use. We need commands now.
In the terminal window, while your device is on, go to Settings on your phone.
Go to About phone.
Scroll down until "Build number" comes in on your ready-to-root vison.
Click it 7 times til' your fingers burn you.
If prompted, enter your screen lock/password.
Go back into the main settings menu.
Find Developer Settings. If you cant find it anywhere, search it!
Go to the Developer Setting menu and scroll until you see USB Debugging.
Turn it on.
If your phone is already plugged into your PC, a menu should pop up. Click Always allow from this computer/device, and click on Allow.
Now, scroll more on the list til' you find OEM unlocking. Turn it on and click on Allow/Okay/Yes if a window appears.
Now, in the terminal window on the PC, run the command as follows: adb reboot bootloader
If your screen turns black on your phone and it reboots to a photo of a Android guy getting fixed, we are getting somewhere.
If it doesn't do ANYTHING at all, please tell me, or follow these steps:
Phone is plugged in
USB Debugging is on
OEM unlocking is on
You didn't install Moto drivers before
etc.
Anyway, if you got this far, run the command as follows: fastboot oem get_unlock_data
If it spits out a stupidly long key, like:
(bootloader) 0A40040192024205#4C4D3556313230
(bootloader) 30373731363031303332323239#BD00
(bootloader) 8A672BA4746C2CE02328A2AC0C39F95
(bootloader) 1A3E5#1F53280002000000000000000
(bootloader) 0000000
We need to put these keys together!
Copy the message "(bootloader) 0A40040192024205#4C4D3556313230
(bootloader) 30373731363031303332323239#BD00
(bootloader) 8A672BA4746C2CE02328A2AC0C39F95
(bootloader) 1A3E5#1F53280002000000000000000
(bootloader) 0000000" as so, and paste it into anything like Word, or Notepad.
Combine the keys by deleting the (bootloader) part , and combining them so it looks like this. (30373731363031303332323239#BD008A672BA4746C2CE02328A2AC0C39F951A3E5#1F532800020000000000000000000000)
Your key will look different because it is a private key, but, do NOT share yours.
Copy the long string (30373731363031303332323239#BD008A672BA4746C2CE02328A2AC0C39F951A3E5#1F532800020000000000000000000000) with your keyboard (ctrl C) or by hi-lighting the key and right clicking, and selecting copy.
Paste the long string into the text box they provide. Click "Can my device be unlocked?"
Accept the legal agreement if asked.
If you get a error like "This device can't be unlocked" from your browser, your device is one of the AT&T/Total/Verizon/Cricket/TracFone models that cannot, and will not ever be unlocked.
If it goes through, you will get a email with the account you added to the website.
Find the email (may be in junk) and copy the key it spit out on the email.
Run this command in the terminal. fastboot oem unlock UNIQUE_KEY (REPLACE UNIQUE_KEY WITH THE KEY IT GAVE YOU IN THE EMAIl!)
Now the device will say something. Like "omg dude like dont unlock it you have brain issues" but follow it and use the VOL. keys to select the options.
The device will most likely reboot, and come up with a warning symbol. Click the power button 2 times to boot the device. You have to do this every time the device reboots, just click the button 2 times.
Congrats! The bootloader is unlocked!

3. ROOTING!!!
Finally, we can ROOT the phone. Download Software Fix (https://download.lenovo.com/consumer/mobiles/software_fix_v7.4.2.13_setup.exe). This lets us download files for Magisk, is made by Motorola, and lets us flash Magisk 😎

