# Portable Retro Gaming Console

## Brief Description

  This repository will walk you through using recalbox and a raspberry pi zero to create a handheld gaming console. This console is essentially a battery powered controller that can be plugged into any hdmi compatible device to enjoy a classic gaming experience.

## Step 1: parts

The most important thing to do before attempting to build this is gaining all the correct parts needed.

* Raspberry Pi Zero W
  * aquire here https://www.raspberrypi.org/products/, amazon or ebay also work, find a kit that comes with a mini hdmi to hdmi adapter
* Buttons
  * aquire here https://www.amazon.ca/Tactile-Tact-Push-Button-Switch/dp/B008DS1F6E/ref=sr_1_14?ie=UTF8&qid=1513575037&sr=8-14&keywords=tactile+push+button (you want tall buttons so they can poke through the  
* MicroSD card
  * aquire here https://www.amazon.ca/SanDisk-microSDHC-Standard-Packaging-SDSQUNC-032G-GN6MA/dp/B010Q57T02/ref=sr_1_1?s=pc&ie=UTF8&qid=1513575422&sr=1-1&keywords=micro+sd+card
* Double A Battery Holder 
  * aquire here https://www.amazon.ca/Gikfun-Plastic-Battery-Storage-Arduino/dp/B0156C57OK/ref=sr_1_1?s=electronics&ie=UTF8&qid=1513575520&sr=1-1&keywords=AA+battery+holder
* Small plastic container
  * aquire at a local dollar store
* Perf Board, use stripped perf board instead if you can
  * buy here https://www.amazon.ca/Haobase-Finished-Prototype-Circuit-Breadboard/dp/B015X8KAYO/ref=sr_1_1?s=electronics&ie=UTF8&qid=1513577127&sr=1-1&keywords=perf+board
* Slide switch
  * aquire here https://www.amazon.ca/20pcs-Black-Switch-Electronic-Projects/dp/B00BIAVQSG/ref=sr_1_1?s=hi&ie=UTF8&qid=1513577574&sr=1-1&keywords=small+slide+switch
  
## Step 2: Assembly

  1. download recalbox from https://www.recalbox.com/
  2. download etcher from https://etcher.io/
  3. Put your micro sd into your computer using an adapter if needed
  4. launch etcher, select the recalbox for your img file and the micro sd card for the destination
  5. Selet flash and let etcher do its thing, if it needs to format the drive, format the drive
  6. Take your 4 double A battery holder, strip the ends of the wire and solder to the bottom of the power in micro usb with ground being the outer most solder pad. Your positiv end should connect to a slide switch in the middle, and from one of the sides to the positive of the raspberry pi.
  7. Watch https://www.youtube.com/watch?v=bhWTfATkg6w&t=349s at 4 minutes, this is how we will do our buttons, but where he uses rubber pads we will solder our tactile buttons on.
  8. solder you common ground to a ground pin and solder your buttons appropriatley according to F9SYXD7IUSM1CEG.SMALL.jpg
  9. take your plastic case and mark where the button holes need to be drilled out with a dry erase marker. Also mark where your switch will go
  10. drill and cut holes appropriately, clear space in case where needed
  11. attach your micro hdmi to hdmi adapter, fit you components in the case and hot glue together
  12. launch your console and plug in a usb keyboard for the first launch
  13. your raspberry pi zero w will have wifi capabilities so press enter on the keyboard then navigate to and fill out your wifi settings, take note of the ip address you obtain
  14. download winscp at https://winscp.net/eng/download.php
  15. launch winscp, add a connection to the ip address you got, username: root, password: recalboxroot
  16. navigate to recalboxshare/system/recalbox.conf
  17. enable gpio controls in there and save
  18. launch kodi media center on you console
  19. on the same computer type the ip into a browser url bar
  20. got to the roms tab to add emulators and other games to the console
  21. that's it, the project is done adter restarting recalbox should work with the gpio buttons you made


